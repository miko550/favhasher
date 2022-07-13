# favhasher
Calculate Favicon Hash for Shodan

## Setup
```
git clone https://github.com/miko550/favhasher.git
cd favhasher
pip3 install -r requirements.txt
```
## Usage
```
usage: favhasher.py [-h] [-t TARGET] [-l LIST]

optional arguments:
  -h, --help            show this help message and exit
  -t TARGET, --target TARGET
                        The hostname of the target, eg: github.com
  -l LIST, --list LIST  List of target url saperated with new line
```
## Example
```
└─$ python3 favhasher.py -t github.com     

url:https://github.com/favicon.ico
http.favicon.hash:1848946384

└─$ python3 favhasher.py -l test.txt

url:https://github.com/favicon.ico
http.favicon.hash:1848946384

url:about.gitlab.com
http.favicon.hash:not found

url:https://twitter.com/favicon.ico
http.favicon.hash:-1831547740
```
