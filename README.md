Cite Reference
----------
Author: https://github.com/ethanXWL
Title of program/source code: Python-Selenium-Facebook-group-auto-poster
Code Version: Commit Version 2cd2aab9ae9f4195dbc6553b927f0398e54cc8dc
Type: Source Code
URL: https://github.com/ethanXWL/Python-Selenium-Facebook-group-auto-poster 


# Python-Selenium-Facebook-group-auto-poster
A Python script use Selenium to achieve automatically posting images with text on multiple Facebook groups that you are the member of.

Setup
----------
 - Change facebook setting: 
   1> change to [classic view](https://www.facebook.com/help/645404059595478)
   2> [Disable 2 step authetnication](https://www.alphr.com/facebook/1006409/two-factor-authentication-2FA-facebook)

 - First of all, install [Python 3](https://www.python.org/downloads/) into your machine. I used python 3.7

 - Install [PIP](https://ahmadawais.com/install-pip-macos-os-x-python/)
  
 - Then insall selenium:
   ```
   pip install selenium
   ```
   OR
   ```
   pip3 install selenium
   ```	

 - Check [version of google chrome](https://www.businessinsider.com/what-version-of-google-chrome-do-i-have). I used chrome version 83.0.4103.97.

 - Download the [Chrome Driver](http://chromedriver.storage.googleapis.com/index.html) and place it in the same directory with the script. Make sure chromedriver is same version as google chrome.
   I used [Link](http://chromedriver.storage.googleapis.com/index.html?path=83.0.4103.39/)



Configure the script
----------
You need to edit the script to provide your Facebook account name and password, the message you want to post, whether you want to attach an image, along with its path and the links of the Facebook groups you are the member of:
``` 
def main():
    # Set up Facebook login account name and password
    account = "sample@gmail.com"
    password = "sample"

    # Set up Facebook groups to post, you must be a member of the group
    groups_links_list = [
        "https://www.facebook.com/groups/sample1", "https://www.facebook.com/groups/sample2"
    ]

    # Set up text content to post
    message = "Checkout an amazing selenium script for posting automaticaaly on Facebook groups! https://github.com/ethanXWL/Python-Selenium-Facebook-group-poster"

    # Set up paths of images to post
    images_list = ['C:/Users/OEM/Pictures/sample1.jpg','C:/Users/OEM/Pictures/sample2.jpg']
 ```

#Run
source setup.sh

Running script
---------
After that run the script by runing 

python3.7 fb-group-poster.py 
