# Workshop KIND

## Instalación de herramientas para el workshop

### 1. Instalar Docker

> [docs.docker.com/desktop](https://docs.docker.com/desktop "Docker Desktop Docs")

### 2. Instalar el CLI de herramientas de k8s: kubectl

#### Linux

```bash
sudo apt-get install apt-transport-https ca-certificates curl
```
```bash
sudo curl -fsSLo /usr/share/keyrings/kubernetes-archive-keyring.gpg https://packages.cloud.google.com/apt/doc/apt-key.gpg
```
```bash
echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list
```
```bash
sudo apt-get update && sudo apt-get install kubectl
```

#### Mac

```bash
brew install kubectl
```
ó
```bash
brew install kubernetes-cli
```

> más info: https://kubernetes.io/docs/tasks/tools/

### 3. Instalar Kind

#### Linux
```bash
curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.11.1/kind-linux-amd64
chmod +x ./kind
mv ./kind /some-dir-in-your-PATH/kind
```

#### Mac
```bash
brew install kind
```

> más info: https://kind.sigs.k8s.io/docs/user/quick-start/#installation


