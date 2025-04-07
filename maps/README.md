# FAST-LIO Maps

This directory contains 3D point cloud maps generated using FAST-LIO SLAM on a Jetson Xavier NX with a Livox Mid-360 LiDAR.

## Map Files

- **scans.pcd**: The raw point cloud map in PCD format generated directly by FAST-LIO
- **scans.ply**: The same map converted to PLY format for easier visualization in tools like CloudCompare

## Map Generation Details

These maps were created by running FAST-LIO in a lab environment. The mapping process involved:

- Hardware: Jetson Xavier NX + Livox Mid-360 LiDAR
- Environment: Indoor laboratory space
- Mapping duration: Approximately 15 minutes

## Viewing the Maps

### Using PCL Tools
```bash
# Install PCL tools if needed
sudo apt install pcl-tools

# View PCD file
pcl_viewer scans.pcd
