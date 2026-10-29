How to Install Google Chrome Stable on Debian
sudo apt update && sudo apt install -y ca-certificates curl gpg
curl -fsSL https://dl.google.com/linux/linux_signing_key.pub | sudo gpg --dearmor -o /usr/share/keyrings/google-chrome.gpg   

Install Prerequisites and Import the Signing Key:
``code
