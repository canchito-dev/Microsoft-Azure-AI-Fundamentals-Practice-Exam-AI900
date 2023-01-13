# Explore computer vision

## Analyze images with the Computer Vision service
1. You want to use the Computer Vision service to analyze images. You also want to use the Language service to analyze text. You want developers to require only one key and endpoint to access all of your services. What kind of resource should you create in your Azure subscription?
- [ ] Computer Vision
- [ ] Cognitive Services
- [ ] Custom Vision
 
<details>
  <summary>Check your answer</summary>

- [ ] Computer Vision - Incorrect. This resource type only supports image analysis. A separate Language resource (with its own key and endpoint) would be required for text analytics.
- [x] Cognitive Services - Correct. A Cognitive Services resource supports both Computer Vision and Language.
- [ ] Custom Vision - Incorrect. The Custom Vision service is for image classification and object detection, and does not support image analysis or text analysis.
</details>

2. You want to use the Computer Vision service to identify the location of individual items in an image. Which of the following features should you retrieve?
- [ ] Objects
- [ ] Tags
- [ ] Categories

<details>
  <summary>Check your answer</summary>

- [x] Objects - Correct. Computer Vision returns objects with a bounding box to indicate their location in the image.
- [ ] Tags - Incorrect. Tags indicate the items in an image, but not their location.
- [ ] Categories - Incorrect. Categories provide suggested categorizations for the image as a whole, not individual items in it.
</details>

3. You want to use the Computer Vision service to analyze images of locations and identify well-known buildings. What should you do?
- [ ] Retrieve the objects in the image.
- [ ] Retrieve the categories for the image, specifying the celebrities domain
- [ ] Retrieve the categories for the image, specifying the landmarks domain

<details>
  <summary>Check your answer</summary>

- [ ] Retrieve the objects in the image - Incorrect. The objects might identify buildings as buildings, but not a specific well-known landmark.
- [ ] Retrieve the categories for the image, specifying the celebrities' domain - Incorrect. The celebrities domain includes well-known people, not buildings.
- [x] Retrieve the categories for the image, specifying the landmarks' domain - Correct. The landmarks domain includes many well-known buildings around the world.
</details>

## Classify images with the Custom Vision service

4. You plan to use the Custom Vision service to train an image classification model. You want to create a resource that can only be used for model training, and not for prediction. Which kind of resource should you create in your Azure subscription?
- [ ] Custom Vision
- [ ] Cognitive Services
- [ ] Computer Vision

<details>
  <summary>Check your answer</summary>

- [x] Custom Vision - Correct: When you create a Custom Vision resource, you can specify whether it is to be used for training, prediction, or both.
- [ ] Cognitive Services - Incorrect: A Cognitive Services resource can be used by the Custom Vision service for both training and prediction.
- [ ] Computer Vision - Incorrect: The Computer Vision service does not support the training of a custom image classification model.
</details>

5. You train an image classification model that achieves less than satisfactory evaluation metrics. How might you improve it?
- [ ] Reduce the size of the images used to train the model.
- [ ] Add a new label for "unknown" classes.
- [ ] Add more images to the training set.

<details>
  <summary>Check your answer</summary>

- [ ] Reduce the size of the images used to train the model - Incorrect: Changing the size of the images is unlikely to improve performance significantly, and reducing them may even lose some resolution and make the model worse.
- [ ] Add a new label for "unknown" classes - Incorrect: Adding an "unknown" label will not improve the accuracy of predictions for the classes you want to identify.
- [x] Add more images to the training set - Correct: Generally, adding more images to the project and retraining the model is likely to improve performance.
</details>

6. You have published an image classification model. What information must you provide to developers who want to use it?
- [ ] Only the project ID.
- [ ] The project ID, the model name, and the key and endpoint for the prediction resource
- [ ] The project ID, iteration number, and the key and endpoint for the training resource.

<details>
  <summary>Check your answer</summary>

- [ ] Only the project ID - Incorrect: The project ID on its own is not enough information to use the published model
- [x] The project ID, the model name, and the key and endpoint for the prediction resource - Correct: To use a published model, you need the project ID, the model name, and the key and endpoint for the prediction resource.
- [ ] The project ID, iteration number, and the key and endpoint for the training resource - Incorrect: You need the model name rather than the iteration number; and the key and endpoint must be for the prediction resource, not the training resource.
</details>

## Detect objects in images with the Custom Vision service
7. Which of the following results does an object detection model typically return for an image?
- [ ] A class label and probability score for the image
- [ ] Bounding box coordinates that indicates the region of the image where all of the objects it contains are located
- [ ] A class label, probability, and bounding box for each object in the image

<details>
  <summary>Check your answer</summary>

- [ ] A class label and probability score for the image - Incorrect: The classes returned by an object detection model are applicable to individual objects in the image, not the image as a whole
- [ ] Bounding box coordinates that indicates the region of the image where all of the objects it contains are located - Incorrect: The bounding boxes returned by an object detection model indicates the location of a single object.
- [x] A class label, probability, and bounding box for each object in the image - Correct: An object detection model predicts a class label, probability, and bounding box for each object in the image
</details>

8. You plan to use a set of images to train an object detection model, and then publish the model as a predictive service. You want to use a single Azure resource with the same key and endpoint for training and prediction. What kind of Azure resource should you create?
- [ ] Cognitive Services
- [ ] Custom Vision
- [ ] Computer Vision

<details>
  <summary>Check your answer</summary>

- [x] Cognitive Services - Correct: A cognitive services resource can be used for both training and prediction.
- [ ] Custom Vision - Incorrect: Creating a Custom Vision resource for both training and prediction results in two separate resources being provisioned, each with their own key and endpoint.
- [ ] Computer Vision - Incorrect: A Computer Vision resource cannot be used to train an object detection model from your own images.
</details>

## Detect and analyze faces with the Face service
9. You plan to use Face to detect human faces in an image. How does the service indicate the location of the faces it detects?
- [ ] A pair of coordinates for each face, indicating the center of the face
- [ ] Two pairs of coordinates for each face, indicating the location of the eyes
- [ ] A set of coordinates for each face, defining a rectangular bounding box around the face

<details>
  <summary>Check your answer</summary>

- [ ] A pair of coordinates for each face, indicating the center of the face
- [ ] Two pairs of coordinates for each face, indicating the location of the eyes
- [x] A set of coordinates for each face, defining a rectangular bounding box around the face - Correct: The locations of detected faces are indicated by coordinates for a rectangular bounding box
</details>

10. What is one aspect that may impair facial detection?
- [ ] Glasses
- [ ] Extreme angles
- [ ] Fast shutter speed

<details>
  <summary>Check your answer</summary>

- [ ] Glasses
- [x] Extreme angles - Correct: Best results are obtained when the faces are full-frontal or as near as possible to full-frontal
- [ ] Fast shutter speed
</details>


<details>
  <summary>Check your answer</summary>


</details>