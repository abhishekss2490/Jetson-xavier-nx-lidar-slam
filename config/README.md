# Configuration Files

This directory contains the configuration files used for the FAST-LIO SLAM system.

## Files

- **mid360.yaml**: Configuration for FAST-LIO parameters
- **MID360_config.json**: Configuration for the Livox Mid-360 LiDAR driver

## Key Parameters

### FAST-LIO Configuration (mid360.yaml)
- **point_filter_num**: 3 (controls point cloud density)
- **max_iteration**: 3 (optimization iterations for ICP)
- **frame_rate**: 10 Hz
- **extrinsic calibration**: Parameters for LiDAR-IMU calibration

### Livox Driver Configuration (MID360_config.json)
- **IP address settings**: Network configuration for the LiDAR
- **Point cloud type**: Data format settings
- **Scan pattern**: LiDAR scanning pattern configuration

These configuration files are optimized for running on the Jetson Xavier NX with limited computational resources while maintaining mapping accuracy.
