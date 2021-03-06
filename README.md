# Face Anonymization

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)

Python CLI application that is capable of detecting faces and anonymizing it. 
Face blurring and anonymization have many practical applications. Some of the include :

 - [ ] In public and private areas, privacy and identity protection are important.
 - [ ] Children's internet safety (i.e., blur faces of minors in uploaded photos).
 - [ ] News reporting and photojournalism (e.g., blur faces of people who did not sign a waiver form).

## Getting Started
### Prerequisites
-   `git`  should be installed (recommended v2.4.11 or higher)
-  `python3` should be installed  (recommended v3.8.1 or higher)
- `pip3` should be installed (recommended v23.1.1 or higher) 

### Installation Steps

1.  First of all you need to setup your virtual environment. (setup and activate)

```
pyvenv-3.6 chtenv
```

Install the python virtual environment setup using this command  `sudo apt install python3.6-venv`

```
source chtenv/bin/activate
```

2.  Install all the dependencies, python modules

```
pip3 install -r requirements.txt
```

3.  Run the python CLI app that shows the needed arguments

To see all available options, run `python3 project.py -h` or `python3 project.py --help`.

<p align="center">
  <img src="https://i.ibb.co/h1ng8VG/h.png" alt="Help Flag"/>
</p>


## System Architecture
<p align="center">
  <img src="https://i.ibb.co/njdhh8Y/temp.png" alt="System Architecture of the system"/>
</p>

## Output
First Let us Consider the cases where we use a pre-recorded video as input.
### Blurred Image
On running `python3 project.py -i test1.mp4`, we get

| Input | Ouput |
| :---: | :---: |
| ![test1 mp4 inp](https://user-images.githubusercontent.com/68915136/144244108-584551ef-470a-487a-b2ca-1eea7b71d8ad.png) | ![test1 mp4 -b](https://user-images.githubusercontent.com/68915136/144244243-fd60d6ae-6bab-420d-9538-988e8ff9e3c4.png) | 

### Pixelated Image
On running `python3 project.py -i test1.mp4 -p`, we get

| Input | Ouput |
| :---: | :---: |
| ![test1 mp4 inp](https://user-images.githubusercontent.com/68915136/144244108-584551ef-470a-487a-b2ca-1eea7b71d8ad.png) | ![test1 mp4 -p](https://user-images.githubusercontent.com/68915136/144244553-769f82c5-fe14-4c11-a199-dead568f45c9.png) | 

### Emoji Masked Image
On running `python3 project.py -i test1.mp4 -m`, we get

| Input | Ouput |
| :---: | :---: |
| ![test1 mp4 inp](https://user-images.githubusercontent.com/68915136/144244108-584551ef-470a-487a-b2ca-1eea7b71d8ad.png) | ![test1 mp4 -m](https://user-images.githubusercontent.com/68915136/144244641-9a2aba86-d866-42a8-95be-a86770989b58.png) |

### Save Processed Video
We can save the processed video with `python3 project.py -s output.mp4`. The video is saved as output.mp4.
 
<p align="center">
  <img src="https://i.ibb.co/zh5mHRL/new-vid.png" alt="Blurred Image from Webcam"/>
</p>

Next let us look at the output when live streamed with a webcam
### Blurred Image
On running `python3 project.py`, we get

<p align="center">
  <img src="https://i.ibb.co/5MpQnvZ/webcam-b.jpg" alt="Blurred Image from Webcam"/>
</p>

### Pixelated Image
On running `python3 project.py -p`, we get

<p align="center">
  <img src="https://i.ibb.co/BZSqMvq/webcam-p.png" alt="Pixelated Image from Webcam"/>
</p>

### Emoji Masked Image
On running `python3 project.py -m`, we get

<p align="center">
  <img src="https://i.ibb.co/7bzMfhM/webcam-m.png" alt="Emoji Masked Image from Webcam"/>
</p>

### Adding Borders
On running `python3 project.py -b`, we can add borders to the area where the face is detected

<p align="center">
  <img src="https://i.ibb.co/sjd7xbr/webcam-border.jpg" alt="Border Flag"/>
</p>

## Contributors

The contributors for this project are :

 - Aditya Anil	
 - Sreerag K Vivek
 - Vivek Haridas
