# SA-C-GENDER-CLASSIFIER
# Algorithm
1.Install deepface

2.Import necessary packages

3.Read the image

4.Analyze the gender using deepface

## Program:
```python
/*
Program to implement Gender Classification
Developed by   : Ajay A
RegisterNumber :  212219040006
*/
#install deepface
pip install deepface


from deepface import DeepFace
import cv2
import matplotlib.pyplot as plt

#read the image
image=cv2.imread('/content/WIN_20220608_20_42_43_Pro.jpg')
plt.imshow(image[:,:,::-1])

gender = DeepFace.analyze(image,actions=['gender'])
age = DeepFace.analyze(image,actions=['age'])
emotion = DeepFace.analyze(image,actions=['emotion'])
print("************************************************")
print("Gender : ",gender['gender'])
print("Age : ",age['age'])
print("Emotion :",emotion["emotion"])
print("************************************************")
```

## OUTPUT:

1. CODE :

![Screenshot (7)](https://user-images.githubusercontent.com/102233600/172661949-1b1ef1e2-d43d-4d10-9ab6-56b4ab653b65.png)


2. DEMO VIDEO YOUTUBE LINK:
https://youtu.be/D_tuvU5miNQ
