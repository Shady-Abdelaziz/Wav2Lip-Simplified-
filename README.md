## Wav2Lip-Simplified 

# The main author and repository is https://github.com/Rudrabha/Wav2Lip

This repository contains a simplified implementation of the Wav2Lip project. The instructions below will guide you on how to set up and run the code.

 Requirements

- Python 3.x
- Git
- wget
- ffmpeg
- Additional Python packages (specified in the `requirements.txt` file)

 Setup Instructions

 Step 1: Clone the Repository and Install Dependencies

```
 Remove any existing sample data directory
rm -rf /content/sample_data
mkdir /content/sample_data

 Clone the Wav2Lip repository
git clone https://github.com/zabique/Wav2Lip

 Change directory to Wav2Lip and install the required packages
cd Wav2Lip
pip install -r requirements.txt
```

## Step 2: Download Pretrained Models

download the main models from here https://github.com/Rudrabha/Wav2Lip

## Step 3: Install Additional Dependencies
```
pip install ffmpeg-python mediapipe==0.9.1
pip install ffmpeg-python
pip install librosa==0.9.1
```

## Step 4 : Start syncing
```
python inference.py --checkpoint_path checkpoints/wav2lip_gan.pth --face "/content/sample_data/input_video.mp4" --audio "/content/sample_data/input_audio.wav"
```


