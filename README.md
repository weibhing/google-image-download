# Google Image Downloader
Scrapes images from Google Images using pre-defined keywords, image count and image resolution.
 
##Quick Start

###Install
Run the following code to download the code and install the required packages:
```
$ git clone https://github.com/weibhing/google-image-download
$ cd google-image-download
$ pip install -r requirements.txt
```
Please ensure that you are using the correct ChromeDriver version as installed in your PC.
ChromeDriver link: https://chromedriver.chromium.org/
The ChromeDriver.exe must be located in the same directory as the script.


### Usage
Run the following python script:
```
py search_and_download.py -s KEYWORD [KEYWORD ...] \
						-c IMAGE_COUNT \
						-l
optional arguments:
  -h, --help            show this help message and exit
  -s KEYWORD [KEYWORD ...], --search KEYWORD [KEYWORD ...]
                        Provide keyword to be searched in google
  -c IMAGE_COUNT, --count IMAGE_COUNT
                        Provide number of images to be downloaded
  -l, --large           Download higher resolution images (>8MP) (Default: >2MP)							
```
Example usage:
```
py search_and_download.py -s cars
						-c 10
						-l
```
The output will be saved into "./images" folder created in the same directory as the code.
![Imgur](https://imgur.com/a/TnFTRCn)

##Reference
The code is partially obtained from https://towardsdatascience.com/image-scraping-with-python-a96feda8af2d .
Several enhancements have been made on top of the original source code.






