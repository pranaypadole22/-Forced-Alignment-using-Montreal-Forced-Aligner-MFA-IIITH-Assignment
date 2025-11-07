# -Forced-Alignment-using-Montreal-Forced-Aligner-MFA-IIITH-Assignment
Objective  Set up and execute a complete forced alignment pipeline using the Montreal Forced  Aligner (MFA) tool. And to understand how automatic alignment works between speech  audio and phonetic transcription. 

#-Setup Instructions, steps to install MFA, prepare the dataset, and run the alignment 
(with example commands).
1.Install Anaconda
https://www.anaconda.com/products/distribution

2.Create a new conda environment
conda create -n mfa_env python=3.10

3.Activate the environment
    conda activate mfa_env

4.Install MFA (Montreal Forced Aligner)
Using pip inside the activated environment
pip install montreal-forced-aligner

5.Download an acoustic model
MFA requires an acoustic model for alignment.
Download the English acoustic model from MFA resources: https://montreal-forced-aligner.readthedocs.io/en/latest/models.html

6.Download a pronunciation dictionary
    english_us_arpa

7.Prepare the dataset
  IITH ASSIGNMENT 
│
├── corpus
│
├── data
│   ├── transcripts
│   └── wav
│
├── output
│
├── screenshots
│
├── scripts
│
├── run_align.bat
│
└── README.md

8.Test MFA installation
  mfa --version

9.Install Praat for inspecting TextGrid files

EXAMPLE:mfa align dataset/wav mfa_dicts/english_us_arpa mfa_models/english output
