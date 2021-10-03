# Nektool
An esoteric utility for updating static HTML image galleries. ``Imagemagick`` and ``sed`` are both required. Very much inspired by [lb](https://github.com/LukeSmithxyz/lb).

## Usage
Nektool can be used both locally or remotely on your server. It also works with Windows Subsystem for Linux.

- Add ``nektool`` to your system's ``bin`` directory.
- Edit ``/bin/nektool`` and change the ``filepath`` variable to wherever your website files are located.
- Change the ``webdir`` variable to wherever on the website your gallery images are going to be stored.
- Upload your image file to whatever folder on your server you like.
- Navigate to that folder and run ``nektool [PAGENAME] [IMAGEFILE]``
