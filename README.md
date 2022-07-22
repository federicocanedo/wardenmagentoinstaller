# Warden Magento Installer
Creates a Magento 2 installation automatically

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

## TO-DO

    - Nothing, the script is perfect already
    - Install opayo automatically with the -o argument
    - Install mailchimp automatically with the -m argument
    - Create a menu so you can install ngrok on an already existing magento installation
    - Fix bug with setup command on magento 2.1