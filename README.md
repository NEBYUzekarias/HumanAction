#            HumanActionRecognitioon
# Requirements
This code requires you have Keras 2 and TensorFlow 1 or greater installed. Please see the requirements.txt file. To ensure you're up to date, run: 

`pip install -r requirements.txt`


You must also have ffmpeg installed in order to extract the video files. If ffmpeg isn't in your system path (ie. which ffmpeg doesn't return its path, or you're on an OS other than *nix), you'll need to update the path to ffmpeg in data/2_extract_files.py.



#Getting the data
First, download the dataset from UCF into the data folder:

`cd data && wget http://crcv.ucf.edu/data/UCF101/UCF101.rar`

Then extract it with unrar e UCF101.rar.

Next, create folders (still in the data folder) with mkdir train && mkdir test && mkdir sequences && mkdir checkpoints.

Now you can run the scripts in the data folder to move the videos to the appropriate place, extract their frames and make the CSV file the rest of the code references. You need to run these in order. Example:

`python 1_move_files.py`

`python 2_extract_files.py`

