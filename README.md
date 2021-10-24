# ShadowFBrute
This easy to use, but yet powerful script will brute force logins on Facebook using a list of passwords. Every wrong attempt will change the proxy used, and every 5 attempts Cookies and Headers.

![SFB](https://user-images.githubusercontent.com/76797159/138580401-31772d43-b587-448e-800d-feb317dfb23c.png)
![SFB](https://user-images.githubusercontent.com/76797159/138580411-3dd88d9a-5b4c-40be-86e6-74a29868b464.png)


# Screenshots


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
You can ignore the -l (log) argument.
```bash
python3 sfb.py -u <Email or Phone#> -p <UrPassList.txt> -l <Name_ur_Log_File>
```
{To use a single password}
```bash 
python3 sfb.py -u <Email or Phone#> -sp <ThePassword> -l <Name_ur_Log_File>
```
{To get help message}
```bash
python3 sfb.py -h
```


# Disclaimer
THIS REPOSITORY AND SCRIPTS INCLUDED IN IT IS FOR EDUCATIONAL, TESTING, AND RESEARCH PURPOSES ONLY! THE OWNER/CREATOR NOR ANY CONTRIBUTOR IS NOT RESPONSIBLE FOR YOUR ACTIONS.
