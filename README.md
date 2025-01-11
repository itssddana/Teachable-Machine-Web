# Teachable-Machine-Web
### Overview:
This project uses a Teachable Machine model to detect images, specifically focusing on identifying a "Cat" through a webcam feed. The model is integrated into a web application, where real-time predictions are made as the webcam captures images.

### Key Features:
Webcam Integration: The application starts the webcam to capture images and process them through the Teachable Machine model.
Prediction Display: It predicts the object class and shows the confidence level (probability) for each class in real-time.
Detection Counter: A counter increments each time the model detects a "Cat" with a probability higher than 50%.
Background Color Change: When a "Cat" is detected, the background color of the webpage changes to light green for visual feedback.
Reset Functionality: There is a button to reset the detection counter and restore the original background color.
Exit Button: The application has an exit button that asks for confirmation before closing the window.

### steps:
Added necessary JavaScript libraries: I included TensorFlow.js and Teachable Machine Image libraries to enable model loading and webcam interaction.

Designed the HTML page: I created a page with buttons for starting the webcam, resetting the counter, and exiting. I also added a section to display webcam feed and prediction results.

Loaded the model: I loaded the Teachable Machine model and metadata using their URLs to prepare for predictions.

Processed predictions: I processed the predictions, specifically looking for the "Cat" class with a probability greater than 50%.

Changed background on detection: When "Cat" is detected, I incremented the detection counter and changed the background color to light green.

Reset the counter: I added a function to reset the detection counter and restore the background to its original color.

Exit functionality: I implemented an exit button that prompts the user for confirmation before attempting to close the page.

Prevented multiple detections: I used a variable to track the previous prediction and avoided counting multiple detections of the same class consecutively.

### Purpose: 
The project is a demonstration of real-time image classification using a pre-trained Teachable Machine model, along with interactive features like detection counters and dynamic UI changes.
