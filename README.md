# Drishti---For-Blind
A smart Assistant for Navigation and go-to text Reading for blind

Drishti helps to read the text in front of the user,
and it also conveys the environment around the visually impaired, by describing the
objects and relationship b/w the objects. Examples are a 'person sitting on a bench,' 'a
dog is sleeping,' 'a stop sign on the road'. On users command the image is captured
with a camera connected to the raspberry pi. If the user wants text description of the
image, the image is analysed by Google's Cloud Vision API using Optical Character
Recognition to detect the characters, letters in the picture, and if the user wants the
scene description of the nearby environment, the image is sent to the Microsoft
Cognitive Services to analyse the image using Computer Vision. Generated result is
stored in the Dynamo DB (Cloud database). When the user asks Alexa to 'Read the
text' or 'Explain the environment', the Alexa Skill Kit triggers AWS Lambda Function to
fetch the results from the database (Dynamo Db). The Alexa app then recites the
stored result on the user's mobile. This innovative device, designed to serve the
visually impaired, is handy, easy to use with high accuracy.
