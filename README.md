# Nektool
An esoteric utility for updating static HTML image galleries. ``Imagemagick`` and ``sed`` are both required.

## Usage
I primarily designed this tool to be used remotely on a server, but can also be configured to run locally if you prefer editing offline.

- Add ``nektool`` to your system's ``bin`` directory.
- Edit ``/bin/nektool`` and change the two variables to reflect where your website files are.
- Make sure that your target webpage has the ``<!-- Gallery -->`` marker wherever you want your images to appear.
- Upload an image to whatever folder you like. I personally do ``/home/USER`` or ``/root`` for the sake of convenience. Navigate to that folder and run ``nektool [PAGENAME, NO .HTML] [IMAGEFILE, NO SPACES]``. By default this creates a thumbnail in ``/img/[PAGENAME]/thumbs``, and moves the image file to ``/img/[PAGENAME]``.

## Disclaimer
This is my first time writing a Shell script, and I'm a complete dingus at it. You're gonna have to ``mkdir`` all your image directories, otherwise it's gonna complain that the directory doesn't exist. I've also mentioned that your image's filename cannot have any spaces, otherwise it's gonna assume you're using more than two arguments and mess everything up. Yes, I've even tried using quote marks and it still messes up. If anyone can help make this script more idiot-proof, feel free to start a pull request.
