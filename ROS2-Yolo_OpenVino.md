Wkwkwk oke, aku perbaiki formatnya! Ini versi yang **bener**:

***

## **README.md**

Simpan file ini di `~/ros2ws/README.md`:

```markdown
# YOLO + OpenVINO + ROS 2

Deteksi objek underwater (baskom & flares) dengan YOLO dan ROS 2.

## Installation

```
cd ~/ros2ws
colcon build
source install/setup.bash
```

## How to Run

**Terminal 1:**
```
source ~/ros2ws/install/setup.bash
ros2 run opencv_masking masking_node
```

**Terminal 2:**
```
source ~/ros2ws/install/setup.bash
ros2 run yolo_openvino yolo_node
```

**Terminal 3:**
```
rqt
# Select: /detected_image
```

**Terminal 4:**
```
ros2 topic echo /object
```

## Topics

- `/raw_image` - Gambar asli
- `/mask_image` - Gambar masking
- `/detected_image` - Gambar dengan bounding box
- `/object` - Text deteksi

## Troubleshooting

```
cd ~/ros2ws
rm -rf build install log
colcon build
source install/setup.bash
```

---

**Author:** Yuwand | **Date:** Nov 18, 2025
```
