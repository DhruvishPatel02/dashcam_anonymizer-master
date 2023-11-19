# dashcam_anonymizer-master

This repository blurs human faces and license plates in images using YOLOv8 as the object detection model and is fine tuned on data from https://storage.googleapis.com/openimages/web/index.html.

Further more for testing and purposes, the real life data is collected from https://idd.insaan.iiit.ac.in/.

## To run the repository

1. First git clone the repository.
```
https://github.com/DhruvishPatel02/dashcam_anonymizer-master
```

2. Create a virtual environment
```
conda env create -f environment.yml
conda activate dashanon
```

3. To blur the images provided in the images folder execute the command
```
python blur_images.py --config configs/img_blur.yaml
```

4. The results will be stored in the directory `blurred_images`

5. To re-run the application, please delete the `run` directory and the `annot_txt` directory.

## Troubleshooting the issues

1. If you face any issues with creating a virtual environment, you can simply install the `OpenCV` and the `Ultralytics` libraries.

```
pip install opencv-python
```

```
pip install ultralytics
```

2. The blur_videos is still in progress and to use those, you can create a `videos` directory and add the videos with extension `.mp4` and rename the videos as `1.mp4, 11.mp4, etc.`

## Authors

Dhruvish Patel

Melika Ahmadi Ranjbar

Mohammad Ali Farahat