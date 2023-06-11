# Human Photo Dancing
This repo is a simple example of how to create a dancing video(.gif) from a single human photo.

## Reference
The following repos are referenced in this project:
- [Animated drawing](https://github.com/facebookresearch/AnimatedDrawings)
- [DIS](https://github.com/xuebinqin/DIS)
- [MMPose](https://github.com/open-mmlab/mmpose)

## Requirements
- Python 3.10 with anaconda
### Prerequisites
- MMPose:
    Please refer to [installation.md](https://mmpose.readthedocs.io/en/latest/installation.html) for more detailed installation
- DIS:
    ```bash
    pip install -r requirements.txt
    ```
- Animated drawing:
    ```bash
    pip install -e .
    ```

## Inference
### 1. go to examples folder
```bash
cd examples
```
### 2. download pretrained model for Pose estimation
you can download the pretrained model from [here](https://mmpose.readthedocs.io/en/latest/model_zoo/body_2d_keypoint.html) and put it in the examples folder
- choose the model you want to download for it's Arch and ckpt
- check the Arch(.py)'s _base_ path is correct. If not, change it to the correct path : ./_base_/

### 3. run the inference
```bash
python image_to_animation.py [human photo path] [output_path]
```
- output path: the path of the output video(.gif)
