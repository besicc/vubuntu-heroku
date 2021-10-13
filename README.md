# Ubuntu-Desktop-noVNC-Heroku-VPS

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?template=https://github.com/akuhnet/hero-vps-lifetime)

Ubuntu-Desktop-noVNC-Heroku-VPS serves docker VPS via heroku web and noVNC


Keep Running Heroku VPS 24/7


[Keep Me VPS Running](http://kaffeine.herokuapp.com/)


My Website

[Akuh.net](https://www.akuh.net/)


Original Repo
[vital987](https://github.com/vital987/vubuntu)


[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?template=https://github.com/akuhnet/hero-vps-lifetime)

## docker
```

apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release \
    
 ```
 
  ```
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg && \
    echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null && \
  apt update && \
  apt install docker-ce docker-ce-cli containerd.io && \
    
 ```
 may
 
  ```
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg && \
    echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu stable main" |tee /etc/apt/sources.list.d/docker.list && \
  apt update && \
  apt install docker-ce docker-ce-cli containerd.io && \
    
 ```
## removed
``` #VS Code
	wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg && \
	install -o root -g root -m 644 packages.microsoft.gpg /etc/apt/trusted.gpg.d/ && \
	sh -c 'echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/trusted.gpg.d/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" > /etc/apt/sources.list.d/vscode.list' && \
	rm -f packages.microsoft.gpg && \
	apt install apt-transport-https && \
	apt update && \
	apt install code -y && \
	cd /usr/bin && \
#Brave
	curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg && \
	echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg arch=amd64] https://brave-browser-apt-release.s3.brave.com/ stable main"|tee /etc/apt/sources.list.d/brave-browser-release.list && \
	apt update && \
	apt install brave-browser -y && \   ```
