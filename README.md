# Automatic-Speech-to-Sign-Language-Translation
A Deep Learning NMT Transformers approach for text to gloss translation and GAN implementation for realistic video generation.

Step 1 : Speech to text conversion
Sample speech files are available in the “sample audio inputs” folder with .wav extension.
Upload the “speech-to-text-382212-46fc5777a765.json” google credentials to activate the Google API.
This step outputs the text from the audio in a variable “audio_to_text”.

Step 2 : Text to gloss translation
The text files and notebook can be accessed from the Transformer Inference folder “https://drive.google.com/file/d/1lg5sh4VHlILvh9SKVxymsAs8PacT_wfr/view?usp=sharing” 
ASLG-PC12 data is available in “aslg_pc12.csv”
“gl_vocab.txt” has gloss vocabulary and “tx_vocab.txt” has text vocabulary.
Saved tokenizer is in “tx_gl_converter”
Saved translation model is in “tx-gl-translator”
This step outputs the gloss translation in a variable “gloss_text”

Step 3 : Pose extraction from videos
The videos from ASLLVD dataset are downloaded from “http://vlm1.uta.edu/~athitsos/asl_lexicon/”
Using the Openpose pose estimation the poses are extracted for the videos from ASLLVD in code “gloss_to_pose_mapping.ipynb” and stored in “lookup” folder as mov

Step 4 : Gloss to Pose mapping
The “lookup” folder has the pose videos which can be accessed from “https://drive.google.com/drive/folders/1-1lH4Ak8j1olG5QLSgpAabSZj4fyLaqR?usp=sharing”
The “video-metadata.csv” has the lookup mapping for all the glosses to poses from “lookup”.
The video clips based on gloss mappings are stored in the “lookup_gloss_videolist/ lookup_mp4” folder in mp4 format.
The pose video lists as txt and final pose videos merged are saved in “lookup_gloss_videolist”

Step 5 : Pose to Sign Language Video
The pose video is split into frames and stored in “frames/initial” folder
All the frames in “frames/initial” folder are cropped, resized and stored in “frames/test_A” 
We run inference on these cropped frames using “GAN inference” at “https://drive.google.com/file/d/1W2c9i2VbFlD6amk1iHgooZxa5xP0dhwz/view?usp=sharing”
The images hence inferred by GAN are stitched together and saved in the “GAN inference” folder.

