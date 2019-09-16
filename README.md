# Scanta Assistant
Integration of Google Assistant SDK
## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.
First run , git clone https://github.com/samacker77/ScantaAssistant.git
cd ScantaAssistant
### Prerequisites

Python3

### Installing

A step by step series of examples that tell you how to get a development env running

#### Audio Testing
1. Open Terminal and test audio by running the following command
> speaker-test -t wav

#### Mic Testing
1. Open terminal and run the following commands sequentially.
> arecord --format=S16_LE --duration = 5 --rate=16000 --filetype=raw_out.raw
> aplay --format=S16_LE --rate=16000 out.raw





### Configuring a new Python VENV
Run the following commands sequentially
 > sudo chmod +x config_env.sh
 > ./config_env.sh
 > source env/bin/activate
 > mkdir /home/<username>/.config/googleassistant-samples
 > cp client_secret_303436686800-808bo8u3me0o5s5ejifg0fdli1dobeg7.apps.googleusercontent.com.json /home/<username>/.config/googleassistant-samples/device_config.json
  
### Installing dependencies
Run the following commmand

> python3 -m pip install -r requirements.txt

### Updating packages
> python3 -m pip install --upgrade google-assistant-library==1.0.1
> python3 -m pip install --upgrade google-assistant-sdk[samples]==0.5.1
Add additional notes about how to deploy this on a live system

### Generating credentials
> python3 -m pip install --upgrade google-auth-oauthlib[tool]

---
> google-oauthlib-tool --scope https://www.googleapis.com/auth/assistant-sdk-prototype --save --headless --client-secrets client_secret_303436686800-808bo8u3me0o5s5ejifg0fdli1dobeg7.apps.googleusercontent.com.json

### Running the sample
> googlesamples-assistant-pushtotalk --project-id scantaai-124e7 --device-model-id scantaai-124e7-scantaai-tvfx97


## Ask Questions, get answers
