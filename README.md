# Automatic-Speech-to-Sign-Language-Translation
A Deep Learning NMT Transformers approach for text to gloss translation and GAN implementation for realistic video generation.

Step 1 : Speech to text conversion

Step 2 : Text to gloss translation
This step outputs the gloss translation in a variable “gloss_text”

Step 3 : Pose extraction from videos
The videos from ASLLVD dataset are downloaded from “http://vlm1.uta.edu/~athitsos/asl_lexicon/”
Using the Openpose pose estimation the poses are extracted for the videos from ASLLVD

Step 4 : Gloss to Pose mapping

Step 5 : Pose to Sign Language Video
The pose video is split into frames and stored in folder 
We run inference on these cropped frames using “GAN inference” 
The images hence inferred by GAN are stitched together and saved.

Note: 
It is an ongoing project, complete code and documentations will be provided later this year towards the end. Till then we are keeping this open for our reference. No rights are given for open usage of this code.
