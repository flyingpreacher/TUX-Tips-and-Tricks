# How to Install Google Chrome Stable on Debian<br>

## Install Prerequisites and Import the Signing Key:
`sudo apt update && sudo apt install -y ca-certificates curl gpg
curl -fsSL https://dl.google.com/linux/linux_signing_key.pub | sudo gpg --dearmor -o /usr/share/keyrings/google-chrome.gpg`   

## Add the Chrome Repository Source:
`echo "deb [arch=amd64 signed-by=/usr/share/keyrings/google-chrome.gpg] https://dl.google.com/linux/chrome/deb/ stable main" | sudo tee /etc/apt/sources.list.d/google-chrome.list`   

## Update and Install:
`sudo apt update`  
`sudo apt install google-chrome-stable`   
