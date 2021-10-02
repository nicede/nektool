# Nektool
Admittedly inspired by [lb](https://github.com/LukeSmithxyz/lb). An incredibly esoteric utility for updating static HTML image galleries. ``Imagemagick`` and ``sed`` are both required.

## Usage
Upload ``nektool`` to your server's ``bin`` directory and run it in the directory where your target image is:

```
nektool PAGENAME FILENAME_WITH_NO_SPACES
```

The changes will be made to ``PAGENAME.html``. Make sure that ``PAGENAME.html`` has the marker ``<!-- Gallery --!>`` wherever you want your gallery images to be displayed.
