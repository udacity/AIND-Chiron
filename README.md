# AIND Chiron Projects

## Overview
[chiron](https://github.com/udacity/udacity-chiron) is a command line tool forfor submitting certain project files to Udacity.  This repository provides the chiron configuration files specific to the AIND program.


## Usage

1. Activate the udacity environment in Anaconda.

	source activate aind


2. Install the `chiron` package for Anaconda. 

	pip install udacity_chiron


3. Download the tournament submission configuration files for AIND.

	git clone https://github.com/udacity/AIND-Chiron.git


4. Copy your agent file `game_agent.py` (required) and data file `data.json` (optional) to the chiron directory and submit:

	cd AIND-Chiron

	udacity submit isolation

After submitting, you can list all your previous submissions by changing to the chiron project folder and running the command:

	udacity ls isolation

You can pull the zip file and feedback for any submission with the command:

	udacity get <SUBMISSION_ID>

### Authenticating with Google or Facebook

Google and Facebook are difficult to use as identity providers for authentication from the command line. Therefore, we ask you to download a JSON web token from [this link](https://project-assistant.udacity.com/auth_tokens/new), and save it as

 - ~/.udacity-pa/jwt for Mac OSX and Linux or
 - %APPDATA%\udacity-pa\jwt for Windows, where %APPDATA% is an environment variable that will have a value like C:\Users\<username>\AppData\Roaming.

The submission script will read the token from your filesystem so that you do not need to authenticate from the command line.