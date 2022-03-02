# ckad-notes

### Setup Kubernetes on macOS

[Docker, VirtualBox, Minikube, Kubectl]
+ https://matthewpalmer.net/kubernetes-app-developer/articles/guide-install-kubernetes-mac.html

+ Install Docker: https://docs.docker.com/desktop/mac/install/
  brew install --cask docker

+ Install Virtual box
  brew install --cask virtualbox
+ https://osxdaily.com/2019/01/25/uninstall-virtualbox-mac-completely/

+ Install Minikube
+ `curl -Lo minikube https://storage.googleapis.com/minikube/releases/v0.27.0/minikube-darwin-amd64 &&\
  chmod +x minikube &&\
  sudo mv minikube /usr/local/bin/`

+ Install kubectl

minikube delete
rm -rf ~/.minikube

