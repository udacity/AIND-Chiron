## AIND Chiron Projects

# Overview
[chiron](https://github.com/udacity/udacity-chiron) is a command line tool forfor submitting certain project files to Udacity.  This repository provides the chiron configuration files specific to the AIND program.


# Usage

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
