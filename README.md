# Eye-Tracking

The objective of the project is to learn how to analyze and visualize eye-tracking data. The dataset consists of rows (one row per one session and one subject) of raw gaze locations x,y recorded in time. Subjects have multiple rows/samples in the dataset.
The dataset has been recorded in a situation where subjects were shown images and had to indicate if they recognized the image or not. A detailed description of the dataset follows:
----------------------
The dataset is available in CSV format (a text file with one row for every sample) or a Matlab format. Every line is a list of comma separated elements as follows:
sid, known, x1, y1, ....xn, yn
where:
sid - subject identifier (sXX)
known - decision of the subject concerning the observed image (true = recognized imaged, false = did not recognize).
xi - the i-th value of the recorded horizontal eye gaze point (raw data)
yi - the i-th value of the recorded vertical eye gaze point (raw data).
The values for x, y are 0,0 for the point in the center of the screen, positive for the right and lower side of the screen and negative for points on the left or upper side from the center.
The number of values differs for every row! (Because it could take different times for participants to react). Assume sampling rate 1000Hz.

Updated details of the setup: 
Subjects were seated at 450mm from the screen.
There was a 3 x 3 points calibration matrix used, upper left point had coordinates -700, -700, and bottom right 700, 700, center point was at 0,0. (These were not pixels, let's call them units). The physical size of the bounding rectangle for the 3x3 matrix was 195 mm (horizontally) and 113mm vertically.
