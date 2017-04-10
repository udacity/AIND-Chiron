# AIND Chiron Projects

## Overview
Submitting to the Isolation competition is performed using the Udacity Project Assistant command line tool.  This repository provides configuration files specific to the AIND program (currently only used for the Isolation PvP tournament submission).


## Usage

1. Activate the udacity environment in Anaconda.

	source activate aind


2a. If you previously installed the `udacity-chiron` package, remove it:

	pip uninstall udacity-chiron


2b. Install the `udacity-pa` package for Anaconda. 

	pip install udacity-pa


3. Download the tournament submission configuration files for AIND.

	git clone https://github.com/udacity/AIND-Chiron.git


4. Copy your agent file `game_agent.py` (required) and data file `data.json` (optional) to the chiron directory and submit. (You can ignore the console feedback about submitting to the website for review -- that does not apply for the Isolation competition.)

	cd AIND-Chiron

	udacity submit isolation


## After Submitting

After submitting, you can list all your previous submissions by changing to the chiron project folder and running the command:

	udacity ls isolation

You can pull the zip file and feedback for any submission with the command:

	udacity get <SUBMISSION_ID>


### Authenticating with Google or Facebook

Google and Facebook are difficult to use as identity providers for authentication from the command line. Therefore, we ask you to download a JSON web token from [this link](https://project-assistant.udacity.com/auth_tokens/new), and save it as

 - ~/.udacity-pa/jwt for Mac OSX and Linux or
 - %APPDATA%\udacity-pa\jwt for Windows, where %APPDATA% is an environment variable that will have a value like C:\Users\<username>\AppData\Roaming.

 Note: If you get an error after downloading the jwt, try moving it to ~/.ursula/jwt (or %APPDATA%\ursula\jwt for Windows). This error should only occur if you are using the udacity-chiron tool rather than the udacity-pa library (step 2 above).

The submission script will read the token from your filesystem so that you do not need to authenticate from the command line.