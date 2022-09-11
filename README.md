# Licence-plate-recognisation-system
A possible study field in smart cities and the Internet of Things is licence plate realisation or identification using image processing techniques. The use of automated systems to maintain vehicle information for various purposes is required due to the exponential growth in the number of cars.
# Implementation:
An effective approach for recognising Indian car number plates has been developed in the proposed algorithm. We can manage loud, dimly lit, crooked, and number plates with unusual fonts. In the pre-processing stage of this work, several image processing techniques are used, including morphological transformation, Gaussian smoothing, Gaussian thresholding, and the Sobel edge detection method. Following number plate segmentation and border-following contour application, contours are then filtered based on character dimensions and spatial localization. Optical Character Recognition (OCR) is the last step we take to identify the retrieved characters. The database is used to store the identified texts after which they are sorted and made searchable.



The owner's vehicle will be easily recognised in modest institutions, housing societies, and apartments thanks to this project. We can change it even further to make automatic car parking gate which can aloow only the registered vehicle to enter the gate.

As a whole, a series of six primary algorithms are necessary for a License Plate Recognition system to be successful which are:

License PlateLocalization

License Plate Sizing and Orientation

Normalization

Characters Segmentation

Optical character recognition (OCR)

Syntactical /Geometrical analysis [2]

# METHODOLOGY The system is divided into two parts:

Entrance Gate.

Exit Gate.

The entrance is divided into sub-systems which are LCD display system, image acquisition and plate number recognition.

Firstly, the car will stand in front of the barrierthen IR sensor send signal to the microcontroller and it will send message to the matlab,then LCD will display a Welcome Message.

Secondly, the image(license plate) acquired from the hardware components by the Camera will be analyzed in data analysis part where mostly done in Matlab.Then theanalyzed image will be compared with the information stored in the database, if this image is matched with the information stored in the database, then Matlab send massage to the microcontroller to open the barrier gate and after some time delay thebarrier gate will be close again. But if the image doesnt match with any image from those images in the database then ,the Matlab will send a message to the microcontroller, and the microcontroller will turn on alarm and LCD will display amessage you are not allowed to enter, please go back . All the displayed are the output from the microcontroller.

The exit part is very simple compare with entrance, which is when the car stand in front of the barrier, IR sensor send signal to microcontroller and it will open the barrier gate,and after some time delay, the barrier gate will be close again.

SENSORS

Raspberry pi

PI CAMERA

COMPUTER

# CIRCUIT EXPLANATIONS Our project has some parts which are:

INDICATOR

Software program and camera

Sensor section

MOTORS

Indictor section

LCD DISPLAY

Motor section

Display section

# Program is written using Raspberry pi microcontrooler

Start

Repeat

Entrance sensor ==1

NO
YES

LCD displayed (please wait a moment)

Exit sensor

==1

Sent message to python software and wait till got feedback

YES

Open exit barrier wait 10 seconds and close it again

NO

Received message=1

LCD displayed (you are not allow to enter)

YES

Open entrance barrier (stepmotor) waits 10 seconds and close it again

NO

LED indicator light on and off 5 times

NO

LCD displayed (welcome!!)

Entrance sensor ==0

YES

Clear LCD display

End

# Flowchart of License plate recognition steps are:

Open serial port and scan for data.

Load image.

Pre-processing of the image.

LicensePlate Recognition.

Compare with database stored.

Message sent to the microcontroller.
