# Pose Detection

The [Posture Detection on images](./notebooks/posture_detection_on_images_using_mediapipe.ipynb) notebook:

1. Takes in a copy of an original image, then converts the Blue Green Red format to Red Green Blue format as in computer vision which is widely used.

2. Use the `drawing_utils` function to draw all the landmarks points on the image that the model will detect from.

3. Process the pose detection on the converted image format using the process function and perform validation checks whether the landmarks were detected in the image or not. 

4. Draw the landmarks on the image using `draw_landmarks` function (If the landmarks were detected).

5. Display the resultant image.

6. Tests the function `detectPose()` created to perform pose detection on a sample image and display the results.


The [Posture Detection on videos](./notebooks/posture_detection_on_videos_using_mediapipe.ipynb)
notebook:

- Reads an input video frame-by-frame and applies pose detection with the `detectPose()` fuction from the above notebook.


# Workout Detection and Repetition counts on videos.

The [Workout Detection and Repetition counts](./notebooks/Workout_detection_and_repetition_counts_on_videos.ipynb) notebook:

1. Recognizes and classifies poses on images using the K-Nearest Neighbor algorithm. This model was trained with lunges-up-and-lunges-down-images dataset, but can also be trained with other kinds of workout images.

2. Runs a `dump_for_the_app()` function that covert the drawing landmarks of the classified images into a csv file. This csv file is to be used for building pose detection and repetition count application. All credit goes to [WASI AHMED](https://github.com/wasiongit/omdena-workout-project), strong and active collaborator on the Omdena-Singapore-AI-Powered-Workout Project. 

3. Detection and repetiont count on videos.



## Requirements
- pillow
- matplotlib
- numpy
- opencv
- tqdm
- requests
- mediapipe

## Reference
- post detection at https://www.analyticsvidhya.com      

-[WASI AHMED](https://github.com/wasiongit/omdena-workout-project)
