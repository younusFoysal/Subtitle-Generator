# Create env
> python -m venv env

# Activate env
> source env/bin/activate

# Install packages
> python -m pip install ffmpeg faster-whisper ffmpeg-python

> ffmpeg -version


# Freeze packages
> pip freeze > requirements.txt

# TO RUN THE SUBTITLE GENERATOR PROGRAM
1. Create 2 folders
`resources` and `output`
2. Put your input video inside the resources folder
3. Run the below command
> python video_subs.py --input resources/Asset.avi --output output

# TO CONVERT THE SUBTITLE TO SRT PROGRAM
> python subs_convert.py --input output/output.csv --output output

# Deactivate env
> deactivate

# SetUp a new copy of the project
> pip install -r requirements.txt
