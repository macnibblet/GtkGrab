GtkGrab - Screenshot Uploader
================================
Version 0.1.1 Created by Evan Coury


Introduction
------------
GtkGrab is an open source tool for Linux and Mac that takes a screenshot of a window or specified area of the screen, uploads it to a web server of your choice, and copies the URL to your clipboard automatically. Once you start using it, you'll wonder how you got along without it. GtkGrab is essentially a free and open source version of the commercial TinyGrab.com software/service, except that it works on Linux and you don't have to pay to use your own server.

Usage Instructions
------------------
* Press your specified keyboard shortcut.
* On Linux: Either click and drag to specify an area of the screen to capture, or click on the title of a window to capture just that window.
* On Mac: Use the space bar to toggle between mouse and window selection modes.
* Within a few seconds, you should get an unobtrusive notification that your screenshot has been uploaded and that the URL has been copied to your clipboard.

Installation
------------
* Clone your own copy via Git.
* Set a username and password in handler.php and upload it to your server.
* Create a directory called **`caps`** on your server in the same directory as handler.php and chmod it to 777.
* Copy config.cfg-sample to config.cfg. Set the username and password to match handler.php and posturl to be the URL to handler.php.
* Follow any platform-specific instructions below.

Fedora Installation
-------------------
In your terminal, run the following command as root or via sudo:
    yum install scrot ImageMagick xclip
In Gnome, set up a keyboard shortcut for **`GtkGrab/screenshot`** of your choosing via System -> Preferences -> Keyboard Shortcuts.

Ubuntu Installation
-------------------
In your terminal, run the following command:
    sudo apt-get install scrot imagemagick xclip
In Gnome, set up a keyboard shortcut for **`GtkGrab/screenshot`** of your choosing via System -> Preferences -> Keyboard Shortcuts.

Mac Installation
----------------
* Install Growl and growlnotify from http://growl.info/
* Use automator to run **`GtkGrab/screenshot-mac`** via the keyboard shortcut of your choice.

Windows Installation
--------------------
Sorry, GtkGrab does not support your operating system. If anyone would like to add Windows support, please fork the project and let me know!
