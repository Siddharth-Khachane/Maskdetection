# Maskdetection
Median Thresholding For Canny Edge Detection in Mask Detection


Feeding Grayscale images (raw) to the Model was unnecessary as our problem is mask detection and we don't need the exact facial features.  So, I experimented with Edge detection for making the features fed less. I tried various Edge detection methods like Sobel, Canny and found out that Canny Gave me the best results. There was a new Problem as Canny had threshold limits and i had to fix a single threshold upperbound and lower bound for all the images, then it wasn't doing them justice as all images were different and some essential features were lost or some features such as the folds on the mask were tampering with the results. Therefore I implimented the Median method for determining the threshold limits. So each image has different thresholds and thus the Canny Filter applied on it is also unique.

## For further insight, you can refer Understanding.docx
