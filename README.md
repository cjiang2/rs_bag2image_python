# rs_bag2image_python
A Python script to extract RGB and depth frames from a Intel RealSense bagfile. 

## Requirements
- Python 3
- pyrealsense2
- Numpy
- OpenCV

## Usage
```
usage: bag2image.py [-h] [-post_processing [POST_PROCESSING]]
                    [-save_colorize [SAVE_COLORIZE]] [-save_pc [SAVE_PC]]
                    [-visualize [VISUALIZE]]
                    bagfile

Convert bagfile to images.

positional arguments:
  bagfile               Path to bagfile.

optional arguments:
  -h, --help            show this help message and exit
  -post_processing [POST_PROCESSING], --post_processing [POST_PROCESSING]
                        Enable depth post processing.
  -save_colorize [SAVE_COLORIZE], --save_colorize [SAVE_COLORIZE]
                        Save colorized depth map.
  -save_pc [SAVE_PC], --save_pc [SAVE_PC]
                        Save point cloud data.
  -visualize [VISUALIZE], --visualize [VISUALIZE]
                        Visualize while saving.
```
### Output
```
file.bag
file
  |-1_rgb.png
  |-2_rgb.png
  |
  |-1_depth.npy
  |-2_depth.npy
  |
  |...
```
