# NVM
### Install NVM (Node Version Manager):
 ```
 curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
 ```
 * Do not use sudo as it will enable nvm for the root user.
 
 ### Check Version
 ```
 nvm --version
 ```
  ### Check list of all Node.js versions that can be installed with nvm.
  ```
  nvm list-remote
  ```
  
 # NODE JS 
 ### install the latest available version of Node.js
 ```
 nvm install node
 ```
  
### Install two more versions, the latest LTS version and version 14.16.0
```
nvm install --lts
nvm install 14.16.0
```
  
### Get can list the installed Node.js versions
```
nvm ls
```
  
### Change the currently active version
```
nvm use 14.16.0
```
### change the default Node.js version
```
nvm alias default 14.16.0
```

### Change the currently active version
```
nvm use 14.16.0
```



