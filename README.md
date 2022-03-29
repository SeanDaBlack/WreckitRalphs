# WreckItRalphs
[Setup](#setup)\
[Usage](#usage)

Credit to SeanDaBlack for the basis of the script.

main.py is selenium python bot.
# Setup

On mac/pc:

`pip install -r requirements.txt`

This will install `webdriver-manager` to automatically download the correct chrome driver. If you are having issues opening having it open chrome, check https://github.com/SergeyPirogov/webdriver_manager.
LaTeX must also be installed for resume generation. If you're unsure where to start with that, follow the [official instructions](https://www.latex-project.org/get/). (Mac users: I'd recommend using [Homebrew](https://brew.sh/) to install [BasicTex](https://formulae.brew.sh/cask/basictex#default).)

`python main.py` to run. It will loop until you kill the job. `ctrl + c` in your terminal to give HR a break (optional).

Mac:

You might also get a trust issue with the downloaded driver being unverified. To fix that, run 

`xattr -d com.apple.quarantine chromedriver`

this just tells the OS it's safe to use this driver, and Selenium will start working. See https://timonweb.com/misc/fixing-error-chromedriver-cannot-be-opened-because-the-developer-cannot-be-verified-unable-to-launch-the-chrome-browser-on-mac-os/ for more info.

# Usage
```
usage: A script to automate very legitimate applications to kellogg's production plants affected by union strikes
       python3 main.py [-h] [--cloud] [--mailtm]

options:
  -h, --help  show this help message and exit
  --cloud     Puts script in a 'cloud' mode where the Chrome GUI is visible
  --mailtm    Uses mail.tm instead of guerrilla mail by default

Kellogg bad | Union good | Support strike funds
```
