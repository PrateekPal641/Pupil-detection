# Pupil-detection
A program through which you can track you eyes 

First we specify our face extractor and eye extractor
Next we read our image
# Face extraction
We turn our image into a gray image and apply face_casscade to our image and select the biggest face from the faces which are obtained from the face_cascade
# Eye extraction
Similaryly here we turn our image to grey image and extract eye through eye_casscade but here we only find eyes in upper half of the detected face as the algorithm may also specify mouth or chin as eyes sometimes
Next, we simply define our blob detector
# Cut eyebrows 
Thsi function cuts eyebrows from te detected eyes
# blob detector
thsi function erodes and dilutes our image and puts that image into our defined blob detector to obtain blobs
# main
last is our main function where we define our process of capturing reading and output flow.
