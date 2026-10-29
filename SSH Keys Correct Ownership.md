## Linux and macOS:  
### Set correct ownership
`chown $USER ~/.ssh/config`

### Set strict permissions (read/write for owner only)
`chmod 600 ~/.ssh/config`

### Ensure the .ssh directory itself is secure
`chmod 700 ~/.ssh`  


## Common Permission Standards

**Ensure your files adhere to these standard security levels:**  

File/Directory | Recommended Permissions\
`~/.ssh directory	700 (drwx------)`<br>

`~/.ssh/config	600 (-rw-------) or 644 (-rw-r--r--)`<br>

`Private keys (id_rsa)	600 (-rw-------)`<br>

`Public keys (*.pub)	644 (-rw-r--r--)`<br>
