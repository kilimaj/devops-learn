## Docker installation Ubuntu 22.04

- Full list of installation parameters: [see] (https://hub.docker.com/_/jenkins/)

```
sudo apt update && sudo apt upgrade
```

- Installing Docker [instructions](https://docs.docker.com/engine/install/ubuntu/)

```
sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```

```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```

```
echo \
  "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

```
sudo apt update && sudo apt upgrade
```

```
sudo apt-get install docker-ce docker-ce-cli containerd.io
```

- Go back to first page                                                                                            [home](../README.md)