<b>http://askubuntu.com/questions/461943/how-do-i-open-chromium-in-incognito-mode-by-default</b>

I assume you mean the Chromium Web Browser.

You have to change one line in the chromium-browser.desktop file. The best is to do that locally:

Copy the file from /usr/share/applications to /home/yourname/.local/share/applications
Open the file with gedit (open gedit and drag the local desktop file on to the gedit window)
Find the first line in the file that begins with Exec=
Replace the line by Exec=chromium-browser --incognito
a few remarks:

The folder /home/yourname/.local/share/applications is a hidden folder by default. To make it visibe: go to your home folder, type ctrl + h, the .local folder will appear.
You can copy the chromium-browser.desktop file to your local folder with the command: cp /usr/share/applications/chromium-browser.desktop ~/.local/share/applications/chromium-browser.desktop
You might have to log out and back in before the changes to take effect.
