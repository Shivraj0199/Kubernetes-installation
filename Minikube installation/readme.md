## Step 1: Install Docker

```
sudo apt update
sudo apt install -y docker.io
sudo usermod -aG docker $USER
```

## Step 2: Install kubectl (official method)

```
curl -LO "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl"
chmod +x kubectl
sudo mv kubectl /usr/local/bin/
```

## Step 3: Install Minikube

```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```

## Step 4: After Installing, Start Minikube

``` minikube start or minikube start --driver=docker```

## Step 5: Check minikube status

``` minikube status ```

## Step 6: Check nodes

``` kubectl get ndoes ```

