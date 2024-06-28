# Clone the repo
git clone git@github.com:gbrouwer/ml-website.git

# Intall the large file extension from https://git-lfs.com/
port install git-lfs

# Add all files that are big and should bypass commits
git lfs track "*.wav"
git lfs track "*.mp3"
git lfs track "*.aifc"
git lfs track "*.mp4"
git lfs track "*.mov"
git lfs track "*.mov"

# Add the file for tracking them
git add .gitattributes

# Create Environment
python3 -m venv .venv

# Activate the environment
source .venv/bin/activate
