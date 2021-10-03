# Nektool
An esoteric utility for updating static HTML image galleries. ``Imagemagick`` and ``sed`` are both required. Very much inspired by [lb](https://github.com/LukeSmithxyz/lb).

## Usage
Nektool can be used both locally or remotely on your server. It also works with Windows Subsystem for Linux.

- Add ``nektool`` to your system's ``bin`` directory.
- Edit ``/bin/nektool`` and change the two variables to reflect where your website files are.
- Upload your image file to whatever folder on your server you like.
- Make sure that your target webpage has the ``<!-- Gallery -->`` marker wherever you want your images to appear.
- Navigate to that folder and run ``nektool [PAGENAME] [IMAGEFILE]``. Make sure your image's filename has **NO SPACES**. By default this creates a thumbnail in ``/img/[PAGENAME]/thumbs``, and moves the image file to ``/img/[PAGENAME]``.

## Disclaimer
This is my first time writing a Shell script, and I'm a complete dingus at it. You're gonna have to ``mkdir`` all your image directories, otherwise it's gonna complain that the directory doesn't exist. I've also mentioned that your image's filename cannot have any spaces, otherwise it's gonna assume you're using more than two arguments and mess everything up. Yes, I've even tried using quote marks and it still messes up. If anyone can help make this script more idiot-proof, feel free to start a pull request.
