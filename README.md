# Warden Magento Installer
Creates a Magento 2 installation automatically with ✨Warden✨

## Install

- You must first install warden https://docs.warden.dev/installing.html
- Create a directory
- Copy the installmagento python script to this directory

## Pre use

- Warden will use you .composer/auth.json so put your marketplace credentials
- the warden container must be running, so run **warden svc up**

## How to use

- ./installmagento -d domain -v magento-version

    Example: ./installmagento -d test2.4.4 -v 2.4.4

- Optional arguments:

    -s : Will install magento with the sampledata module

    -n ngrok-token : Will setup ngrok for the magento installation, the ngrok url will be printed at the end

- Once the script ends your magento url will be https://app.domain.test (If you didn't use the ngrok argument), if you are on linux you will have to add app.domain.test to /etc/hosts in 127.0.0.1
- It should work on macOS, can't test it properly right now
- The admin page is /admin
- You can edit the basic user config at the bottom of the script, I left my info as an example

## TO-DO

    - Nothing, the script is perfect already
    - Install opayo automatically with the -o argument
    - Install mailchimp automatically with the -m argument
    - Create a menu so you can install ngrok on an already existing magento installation and also make it more ✨User friendly✨
    - Fix bug with setup command on magento 2.1
    - Add more versions to the json file


Based on https://github.com/gonzaloebiz/wardenscripts