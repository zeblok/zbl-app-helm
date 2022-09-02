# Zeblok Helm Charts

## Install Helm Ubuntu
```bash
$ curl https://baltocdn.com/helm/signing.asc | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null
$ sudo apt-get install apt-transport-https --yes
$ echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/helm.gpg] https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
$ sudo apt-get update
$ sudo apt-get install helm
```

# Add Repository
```bash
$ helm repo add zbl-app https://zeblok.github.io/zbl-app-helm/
```

# Install Chart
```bash
$ helm install my-zbl-app zbl-app/zbl-app --version 1.2.1
```

# Check Pods 
```bash
$ kubectl get pods --all-namespaces 
```