# Face_recognition_using_OpenCV
1. Download Raw Images:
Download raw images from Google using any method such as manual downloading, web scraping with Selenium, Chrome extensions, or third-party apps/vendors.

2. Preprocessing and Face Detection:
Use OpenCV (cv2) to read the images and convert them to grayscale using cv2.cvtColor(img, cv2.COLOR_BGR2GRAY).
Utilize Haar cascades classifiers for detecting eyes in the images by analyzing lines and edge features with a moving window approach.
Draw rectangles on the region of interest to identify faces and eyes using OpenCV.

3. Crop Faces and Eyes:
Implement functions to crop the images, focusing on individual faces and extracting two eyes using the detected bounding boxes.

4. Organize Dataset:
Create multiple folders for each individual face, and save the cropped images of faces and eyes in their respective folders.

5. Data Preparation:
Create a dictionary with individual labels and image addresses to organize the dataset.

6. Convert to NumPy Arrays:
Use OpenCV to convert the cropped images into NumPy arrays, which can be fed into the model for training and identification.

7. Model Training and Hyperparameter Tuning:
Use grid search CV algorithm to find the best hyperparameters for the model.

8. Model Testing and Evaluation:
Test the trained model on the validation set and evaluate its performance.
Achieve a best score of 83% accuracy in the final model.

10. Visualization:
Use classification reports and Seaborn library for better visualization of the model's results.
