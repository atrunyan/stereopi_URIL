# stereopi_URIL
Developing repo of stereopi stereovision code 

## calibrate_stereo.py
This script uses the StereoVision library to calibrate stereo cameras. However, the calibration had many issues and wouldn't accurately detect all checkerboards in all photos. Resulting calibration information produced noisy and unclear disparity maps.

## cv_calibrate_stereo.py
A new script to calibrate stereo cameras using openCV. This calibration produces a numpy file with information about the intrinsic/extrinsic properties of the cameras and their rectification. Much more effective calibration than previous script.

## cv_image_disparity.py
This script takes in a left and right image to rectify and produce a disparity map from. Mainly for tuning parameters to use later for stereovideo.
