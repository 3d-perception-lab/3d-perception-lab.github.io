---
title: Tutorials
type: docs
weight: 4
sidebar:
  open: true
---

## 


## Basalt VIO

- basalt_vio target: src/vio.cpp
  - load_data basalt::DatasetIoFactory::getDatasetIo(dataset_type);
  - opt_flow_ptr =
        basalt::OpticalFlowFactory::getOpticalFlow(vio_config, calib);
  -  vio = basalt::VioEstimatorFactory::getVioEstimator(
          vio_config, calib, basalt::constants::g, use_imu, use_double);
  - new basalt::MargDataSaver(marg_data_path)
  - creates VioEstimator from Factory
- src/vi_estimator/vio_estimator.cpp: calls SqrtKeypointVioEstimator in factory_helper
- src/vi_estimator/sqrt_keypoint_vio.cpp: def of SqrtKeypointVioEstimator
  - constructor
  - initialize: 
    - OpticalFlowResult::Ptr prev_frame, curr_frame;
    - collect IMU data corresponding to current frame
    - set vel_w_i_init.setZero(); and T_w_i_init based on accel
    - if prev_frame: 
      - collect all IMU meas, integrate until current frame
      - call "measure" with opt flow result curr_frame
      - prev_frame = curr_frame, push nullptr result
    - finished viofilter init
    - thread reset? 
  - measure:
    - use IMU meas to predict state, input in "frame_states[last_state_t_ns]"
    - Make new residual for existing keypoints
    - decide if take_kf based on number of connected obs (common lm) and config.vio_new_kf_keypoints_thresh
    - if take_kf: triangulate new points
    - do something with lost landmarks
    - optimize_and_marg