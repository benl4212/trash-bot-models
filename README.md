# YOLO Model Files for Trash Bot

## Description

This repository contains pre-trained YOLO11 'nano' model files used by the main project: **[https://github.com/benl4212/trash-bot]**.

These model architectures were developed by Ultralytics and are provided here for convenience, subject to their original license terms.

## Models Included

* **PYTORCH FORMAT MODELS**
* 18 Class `yolov11n.pt`,
* Single Class `yolov11n.pt`, `yolov11n-seg.pt (SiLU)`, `yolo11n-seg.pt (ReLU)`
* **EDGE TPU FORMAT MODELS**
* 18-class `yolov11n_int8_edgetpu.tflite`
  * Imgsz Variants= 540 & 320
* Single Class `yolov11n-seg(SiLU)_int8_edgetpu.tflite`, `yolo11n-seg(ReLU)_int8_edgetpu.tflite`

**NOTE:** yolov11n models include 'box' in the actual file name, while the yolo11n-seg models include 'seg' in the actual file name


## Other Files
* Example data.yaml that describes how the classes were configured for 18-class, and single-class
* EDGE TPU FORMAT ONLY * FILES
  * The .zips also contain a metadata files that show Class Names and Image Size Inputs. Except for the ReLU model because it has identical configurations to SiLU

## Licensing

**IMPORTANT:** The model files contained in this repository are provided under the **GNU Affero General Public License v3.0 (AGPL-3.0)**, as required by Ultralytics, the creators of these models.

Using these models in your own projects requires compliance with the AGPL-3.0 license terms. This generally means that if you distribute software that uses these models, or provide network access to software using these models, you must make the complete corresponding source code of your software available under the AGPL-3.0 license as well.

A full copy of the AGPL-3.0 license text is included in the `LICENSE` file in the root of this repository. You can also find it online here: [https://www.gnu.org/licenses/agpl-3.0.html](https://www.gnu.org/licenses/agpl-3.0.html)

## Acknowledgements

* These models originate from Ultralytics ([https://ultralytics.com/](https://ultralytics.com/)). Please refer to their resources for model details and training information.

## Usage with Main Project

To use these models with the main project **[https://github.com/benl4212/trash-bot]**, download the required model file(s) from this repository and place them in the appropriate directory as specified in the main project's documentation. Remember that by using these models, your usage becomes subject to the AGPL-3.0 license terms.

