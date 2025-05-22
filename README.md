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

My research insights a quick 5mins read:
https://medium.com/@sadakhya/things-to-keep-in-mind-when-training-gan-and-what-i-realized-while-trying-to-improve-my-inference-63291e3ea6fc
