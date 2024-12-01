## iris Segmentation Using "mediapipe" and changing iris color using HSV sepctrum
Iris segmentation is the process of isolating the iris region (the colored part of the eye) from an eye image. This is the first and crucial step in iris recognition systems, where the unique patterns in the iris are used for biometric identification. 
* The CFD Dataset used in this repo

Using mediapipe landmarks and google image which contains the number of landmarks of human face it's possible to segment the left & right eyes.

![image](https://github.com/user-attachments/assets/01ee3a4d-7e1c-4305-a13b-f7f943a8ee9d)

Then using morphological operations to create mask for eyes.
![image](https://github.com/user-attachments/assets/d1fa3cdb-96a2-4c8d-af8c-a1f7c7c85f7d)

For segmenting the exact iris, the method "Hough circle transform" has been used.
* the problem with hough transform is the parameters and for different images, the parameters should be changed
![image](https://github.com/user-attachments/assets/2054623e-c6bb-4d25-891c-3ae31c842371)
![image](https://github.com/user-attachments/assets/67cb88fa-84c5-4e50-a5a7-69bc72c75608)
![image](https://github.com/user-attachments/assets/edaaeda3-e36d-4069-a1bc-0495293578a0)

In the final step converting the RGB format image into HSV to change the hue (and value somehow) to change the iris color.
![image](https://github.com/user-attachments/assets/47b63c66-f1de-42f9-a955-eb7bc18dee37)
##### HSV colors that are appropriate to be used are: [1, 70, 100, 200, 250, 300]

# Initial image:
![image](https://github.com/user-attachments/assets/5c0617a5-bf5d-433c-9d44-2c380e26d404)

# After changing iris color:
![image](https://github.com/user-attachments/assets/3cbf0474-18c3-483f-a3b1-c515c10e15c8)
