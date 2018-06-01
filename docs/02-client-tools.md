# Installing the Client Tools

In this lab you will install the command line utilities required to complete this tutorial: [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl).

## Install vault 

### OS X
```
brew install vault 
```

### Linux
Download the version compatible with your sistem on [documentation](https://www.vaultproject.io/downloads.html)

```
wget https://releases.hashicorp.com/vault/0.10.1/vault_0.10.1_linux_amd64.zip
```

Then
```
unzip vault_0.10.1_linux_amd64.zip && chmod +x vault
```

```
sudo mv vault /usr/local/bin/
```

## Install kubectl

The `kubectl` command line utility is used to interact with the Kubernetes API Server. Download and install `kubectl` from the official release binaries:

### OS X

```
curl -o kubectl https://storage.googleapis.com/kubernetes-release/release/v1.10.2/bin/darwin/amd64/kubectl
```

```
chmod +x kubectl
```

```
sudo mv kubectl /usr/local/bin/
```

### Linux

```
wget https://storage.googleapis.com/kubernetes-release/release/v1.10.2/bin/linux/amd64/kubectl
```

```
chmod +x kubectl
```

```
sudo mv kubectl /usr/local/bin/
```

### Verification

Verify `kubectl` version 1.10.2 or higher is installed:

```
kubectl version --client
```

> output

```
Client Version: version.Info{Major:"1", Minor:"10", GitVersion:"v1.10.2", GitCommit:"81753b10df112992bf51bbc2c2f85208aad78335", GitTreeState:"clean", BuildDate:"2018-04-27T09:22:21Z", GoVersion:"go1.9.3", Compiler:"gc", Platform:"linux/amd64"}
```

Next: [Provisioning Compute Resources](03-compute-resources.md)