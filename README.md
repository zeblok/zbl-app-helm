# Zeblok Helm Charts

## Install Helm Ubuntu
```bash
$ curl https://baltocdn.com/helm/signing.asc | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null
$ sudo apt-get install apt-transport-https --yes
$ echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/helm.gpg] https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
$ sudo apt-get update
$ sudo apt-get install helm
```

# Helm Doc
<a href="https://helm.sh/docs/intro/install"></a>

# Clone Git Repo
```bash
$ git clone https://github.com/zeblok/zbl-app-helm.git
```
# Bash Command 
```bash
$ ls
$ cd zbl-app-helm
$ ls
```

# Git Checkout
```bash
$ git checkout gh-pages
```

# Unzip tgz file
```bash
$ ls
$ tar -xvzf zbl-app-1.2.1.tgz
$ ls
$ cd zbl-app
```

# Install Helm Charts
```bash
$ helm install zbl .
```

# Check Pods 
```bash
$ kubectl get pods --all-namespaces 
```