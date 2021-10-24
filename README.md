# ShadowFBrute
This easy to use, but yet powerful script will brute force logins on Facebook using a list of passwords. Every wrong attempt will change the proxy used, and every 5 attempts Cookies and Headers to prevent blocks.

Tested on:
- Parrot security 4.11.2
- kali-linux 2021.3

Issues:
- Attacking the same account multiple times in a row will result in block giving this error similar to this plus others:
[Python] requests.exceptions.TooManyRedirects: Exceeded 30 redirects or other error
- Solution?
Only attempt to brute force a single account once every hour or so if no password from list isn't found. If you already have errors you'll need to restart and wait as your connection is blocked or reset IP and use a VPN and wait at least 15min to try again. 


# Screenshots
![SFB](https://user-images.githubusercontent.com/76797159/138580401-31772d43-b587-448e-800d-feb317dfb23c.png)
![SFB](https://user-images.githubusercontent.com/76797159/138580411-3dd88d9a-5b4c-40be-86e6-74a29868b464.png)

# Installation & Setup
If you don't already, first get:
- [Python 3](https://www.python.org/downloads/)
- pip

ShadowFBrute:

```bash
git clone https://github.com/shadow-sec/ShadowFBrute.git
```
```bash 
cd ShadowFBrute
```
```bash
pip install -r reqs.txt
```


# Fast Interface Usage
- Open Interface:
```bash
python3 sfb.py
```
---> [?] Password List Filename: sfblist.txt

(You can add passwords to default sfblist.txt found in main folder or add your own .txt file)

---> [?] Email or Phone#: target@email.com or phone-number

Done! Now wait for the results :) Additionally all finished sessions are saved in logging.log with results & other info.

- Command Line Usage:
{To use password list}
You can ignore the -l (log) argument for default logging file.
```bash
python3 sfb.py -u <Email or Phone#> -p <UrPassList.txt> -l <Name_ur_Log_File>
```
{To use a single password}
```bash 
python3 sfb.py -u <Email or Phone#> -sp <ThePassword> -l <Name_ur_Log_File>
```
{To show help message}
```bash
python3 sfb.py -h
```
# Disclaimer
THIS REPOSITORY AND SCRIPTS INCLUDED IN IT IS FOR EDUCATIONAL, TESTING, AND RESEARCH PURPOSES ONLY! THE OWNER/CREATOR NOR ANY CONTRIBUTOR IS NOT RESPONSIBLE FOR YOUR ACTIONS.
