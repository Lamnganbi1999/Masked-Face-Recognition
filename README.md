# Masked-Face-Recognition
## About the Project:
<p> This project uses CNN based Transfer Learning to classify whether a face is masked or not. It uses RESNET-18 Backend with pretrained weights, and customized final layers for Binary Classification (Masked/ Not-Masked).
</p>

## Languages/ Tools used:
<ul>
  <li> Python </li>
  <li> Jupyter Notebook </li>
  <li> Pytorch </li>
</ul>

## Dependencies:
<ul>
  <li> OpenCV </li>
  <li> PILLOW </li>
  <li> Resnet-18 (Architecture + Weights) </li>
  <li> Face_recognition Library </li>
</ul>

## Dataset
RWMFD (Real World Masked Face Dataset)
## Inferences from dataset:
Since the dataset didn't contain accurately cropped image consisting of just the face, face_recognition library was applied on the images, to get closeup cropped images.
<br><br>
<strong> Some examples of closely cropped masked images </strong>
<div><img src = "/Images/masked.png"></div>
<br><br>
<strong> Some examples of closely cropped unmasked images </strong>
<div><img src = "/Images/unmasked.png"></div>

## Training Results
After training for 10 epochs the training loss graphs is as shown below:
<div><img src = "/Images/training.png" ></div>
<br><br>
The validation accuracy is about 97 % after 10 epochs.
<div><img src = "/Images/validation.png" ></div>

## Testing Result
After testing a total of around 150 images, the testing accuracy stands at 97% which can be inferred from the results shown below:

<div><img src = "/Images/result.png" ></div>

## Scopes of Improvement
1. Since the dataset was small, using a large number of images might result in better accuracy.
2. Since the model is dependent on face detection, greater occlusions in face due to mask might be the reason for incorrect prediction sometimes.
3. Face detection module doesn't help identify skewed faces so accurately especially when the size of face is so small. 



