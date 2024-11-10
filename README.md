# EEE_F411_Internet_of_Things
Raspberry Pi Based Facial Recognition with Email Notifications and automated lighting

# Raspberry Pi 4 Facial Recognition
# IOT Project 
# Abhinandan Sharma
# 2018A3PS0095P

Version of RaspberryPi	: 	4b
Version of Python		: 	3.9.2
Version of OpenCV		:	4.5.3

Components used:
	1. Raspberry Pi 4b
	2. USB Webcam
	3. Push button
	4. LAN cable, C type power cable, Jumper wires

Libraries used :
	1. cv2
	2. imutils
	3. face_recognition
	3. pickle
	4. os
	5. time
	6. RPi.GPIO
	7. smtplib
	8. ssl
	9. email

Save this complete Directory by the name of 'Face_recognition' in the pi directory of your raspberrypi	

Open headshots.py and specify the name of the new person to the 'name' variable in lin4
Execute headshots.py
Keep pressing spacebar and images would be clicked and saved in a folder in the 'Datasets' subfolder.
The name of the folder will be same as that specified to the 'name' variable in headshots.py
Any number of images can be taken. I took twenty pics for each person.
We have successfully the collected the dataset which have to be trained !!

Execute train_model.py
All the pics of all the persons will be trained and an encoding file will be created by thr name of encodings.pickle
We have successfully trained the model !!

Execute facial_req.py
The live stream of the USB webcam with a box around all the faces in the frame will be displayed.
Along with the box, the name of the person will also be displayed.
We have successfully performed Facial Identification along with Facial Recognition !!

The python script email_code.py has been imported in facial_req.py
Specify the sender and receiver GMAIL ID along with the password in the script.
Don't forget to switch on the 'Allow less secure apps' feature in the sender gmail ID.
Press the push button at any time and the current frame with the box and name would be captured and saved as image.jpg
This image will be sent via gmail as an attachment the the email ID specified to the 'toaddr' variable.
We have successfully emailed the picture and name oof the new guest !!
