# YOLO Model Files for Trash Bot

## Description

This repository contains custom YOLO11 'nano' model files used by the main project: **[https://github.com/benl4212/trash-bot]**.


These model architectures were developed by Ultralytics and are provided here for convenience, subject to their original license terms.


## Models Included

**PYTORCH FORMAT MODELS**
* 16 Class Model
  * Filenames: `16class_box_pt.zip`
  * Trained from base: `yolov11n.pt`,
* 1 Class Models
  * Filenames: `1class_box_pt.zip` , `1class_seg_relu_pt.zip` , `1class_seg_silu_pt.zip`
  * Trained from bases: `yolov11n.pt`, `yolov11n-seg.pt`
  
**EDGE TPU FORMAT MODELS**
* 16 Class Models
  * Filenames: `16class_box_320_edgetpu.zip` , `16class_box_544_edgetpu.zip`
* 1 Class Models
  * Filenames:`1class_seg_silu_edgetpu.zip`, `1class-seg_relu_edgetpu.zip`

**NOTE:** yolov11n models include 'box' in the actual file name, while the yolo11n-seg models include 'seg' in the actual file name. 
The number (544 or 320) in the file name differentiates the input image size of the model; chosen for testing optimal compilation with 
the [Edge TPU Compiler](https://colab.research.google.com/github/google-coral/tutorials/blob/master/compile_for_edgetpu.ipynb).


## Other Files
* Example data.yaml that describes how the classes were configured for 18-class, and single-class
* EDGE TPU FORMAT ONLY * FILES
  * The .zips also contain a metadata files that show Class Names and Image Size Inputs. Except for the ReLU model because it has identical configurations to SiLU

## Datasets used for Training/Val and PTQ
* Segmentation: [https://universe.roboflow.com/litter-bot/custom-litter-segmentation]
 
* Box: [https://universe.roboflow.com/litter-bot/custom-litter-object-detection]
  
* PTQ: [https://universe.roboflow.com/litter-bot/calibration-set-for-ptq]

## Licensing

**IMPORTANT:** The model files contained in this repository are provided under the **GNU Affero General Public License v3.0 (AGPL-3.0)**, as required by Ultralytics, the creators of these models.

Using these models in your own projects requires compliance with the AGPL-3.0 license terms. This generally means that if you distribute software that uses these models, or provide network access to software using these models, you must make the complete corresponding source code of your software available under the AGPL-3.0 license as well.

A full copy of the AGPL-3.0 license text is included in the `LICENSE` file in the root of this repository. You can also find it online here: [https://www.gnu.org/licenses/agpl-3.0.html](https://www.gnu.org/licenses/agpl-3.0.html)

## Acknowledgements

* These models originate from Ultralytics ([https://ultralytics.com/](https://ultralytics.com/)). Please refer to their resources for model details and training information.

## Usage with Main Project

To use these models with the main project **[https://github.com/benl4212/trash-bot]**, download the required model file(s) from this repository and place them in the appropriate directory as specified in the main project's documentation. Remember that by using these models, your usage becomes subject to the AGPL-3.0 license terms.

