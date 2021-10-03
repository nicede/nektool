# Nektool
An esoteric utility for updating static HTML image galleries. ``Imagemagick`` and ``sed`` are both required. Very much inspired by [lb](https://github.com/LukeSmithxyz/lb).

## Usage
Nektool can be used both locally or remotely on your server. It also works with Windows Subsystem for Linux.

- Add ``nektool`` to your system's ``bin`` directory.
- Edit ``/bin/nektool`` and change the ``filepath`` variable to wherever your website files are located.
- Change the ``webdir`` variable to wherever on the website your gallery images are going to be stored.
- Upload your image file to whatever folder on your server you like.
- Navigate to that folder and run ``nektool [PAGENAME] [IMAGEFILE]``. Make sure your image's filename has **NO SPACES**.

## Disclaimer
This is my first time writing a Shell script, and I'm a complete dingus at it. You're gonna have to ``mkdir`` all your image directories, otherwise it's gonna complain that the directory doesn't exist. I've also mentioned that your image's filename cannot have any spaces, otherwise it's gonna assume you're using more than two arguments and mess everything up. Yes, I've even tried using quote marks and it still messes up. If anyone can help make this script more idiot-proof, feel free to start a pull request.
