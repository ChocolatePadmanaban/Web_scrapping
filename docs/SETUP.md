# Setup web scrapping project 

## Stage 0 : Installed required software packages 

Software packages requried for this project are 
- python3
- selenium python package (which would be inslled from requirement.txt)
- chrome browser (latest)
to update to latest in linux 

```
sudo apt update 
sudo apt --only-upgrade install google-chrome-stable 
```
- chrome selinium web driver 

To install chrome selinium web-driver 
- download latest selinium chrome web-driver which is availabe at this link `https://sites.google.com/chromium.org/driver/`
- which may direct you to a page where wedriver zip files will be listed `https://googlechromelabs.github.io/chrome-for-testing/`
- download the zip file for you chrome version (recommended: update to latest)
```
wget -O chromedriver-linux64.zip "https://storage.googleapis.com/chrome-for-testing-public/<your-version>/linux64/chromedriver-linux64.zip"
```
- unzip the chromedriver zip file 
```
unzip chromedriver-linux64.zip 
```
- move it to bin and make it executable 
```
 sudo mv chromedriver-linux64/chromedriver /usr/local/bin/chromedriver
 sudo chmod +x /usr/local/bin/chromedriver 
```
- check the chromedriver version it should match the latest version 
```
chromedriver --version
```



## Stage 1 : create virtual environment 

- create a virutal environment 

```
python3 -m venv venv 
```
- activate the virtual env 

for linux/macOS
```
source venv/bin/activate
```
for Windows 

```
venv\Scripts\activate
```

- import required libraries from `requirements.txt`

```
pip install -r requirements.txt
```

**Note:** to deactivate the venv after you have done with project just type `deactivate` in terminal 
```
deactivate 
```