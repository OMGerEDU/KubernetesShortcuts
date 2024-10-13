# KubernetesShortcuts
let's admit it, Kubernetes is amazing, but writing 'kubectl logs pod -f' is far more annoying than 'klogv'

Prerequires: 
Kubernetes Command line tool (kubectl) 

How to use?
1. Download the folder, if it's in rar/zip, extract it.
2. Move it to desired location, in Windows, add it in the OS disk.
3. Add the folder to Enviroment variable.
Windows:
enter 'Edit the system enviroemnt variables' in Win Search ->
Enviroment Variable -> Path (System or user variable is your own preference) -> Copy Folder url (in my own case it was C:\cli)

now it should work :) 


# Kubernetes CLI Shortcuts Documentation

This project provides a set of batch scripts to simplify common Kubernetes (kubectl) commands, making it quicker and easier to interact with your Kubernetes cluster. Below is a list of the available scripts and their purposes.

## Script Overview

### 1. `kall.bat`
Displays all resources in the Kubernetes cluster.

```sh
kubectl get all
```
Usage: Simply run `kall.bat` to get all Kubernetes resources.

---

### 2. `kdel.bat`
Deletes all pods in the cluster.

```sh
kubectl delete pods --all
```
Usage: Run `kdel.bat` to delete all pods.

---

### 3. `kdeldep.bat`
Deletes a specific deployment.

```sh
kubectl delete deployment %*
```
Usage: Run `kdeldep.bat <deployment-name>` to delete a deployment by name.

---

### 4. `kdelserv.bat`
Deletes a specific service.

```sh
kubectl delete service %*
```
Usage: Run `kdelserv.bat <service-name>` to delete a service by name.

---

### 5. `kdep.bat`
Gets all deployments in the cluster.

```sh
kubectl get deployments
```
Usage: Run `kdep.bat` to list all deployments.

---

### 6. `kdes.bat`
Describes a specific pod.

```sh
kubectl describe pod %*
```
Usage: Run `kdes.bat <pod-name>` to describe a pod by name.

---

### 7. `klog.bat`
Displays logs for a specific pod.

```sh
kubectl logs %*
```
Usage: Run `klog.bat <pod-name>` to view logs from a pod.

---

### 8. `klogbash.bat`
Opens an interactive bash shell in a specific pod.

```sh
kubectl exec -it %* -- /bin/bash
```
Usage: Run `klogbash.bat <pod-name>` to access the shell in a pod.

---

### 9. `klogv.bat`
[Not fully visible in the snippet, assuming it deals with logging.]

```sh
<kubectl command here>
```
Usage: `<description>`.

---

## Contributing
Feel free to modify or add more scripts to enhance the Kubernetes command-line experience. Contributions are welcome!

## License
This project is open source under the MIT License.

---

These batch scripts are intended to save time and reduce repetitive typing when interacting with Kubernetes clusters. Enjoy managing your Kubernetes resources with minimal hassle!


