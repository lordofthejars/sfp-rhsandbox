# Strangler Fig Pattern Demo @ RivieraDev 🇫🇷 2023

### **0. Prerequisite**

This demo scenario for showcasing the strangler fig pattern **requires access to a Kubernetes cluster**. In case you neither have any locally available k8s environment on your development machine (e.g. `minikube`) nor a Kubernetes cluster playground at your disposal you can can **claim your personal, managed [OpenShift Developer Sandbox](https://red.ht/sandbox4all) free of charge for 30 days** by registering your personal account at Red Hat - NO(!) credit card or any other payment means necessary to do so 😎

### **1. Login to k8s / configure `kubectl`**

Make sure to login / authenticate to the Kubernetes cluster you want to use for running this demo scenario.
Also verify that your `kubectl` is properly configured and points to the cluster in question.

### **2. Run the demo scenario**

In the root directory of the repo you find a bash script which is named `run-sfp-demo.sh`. Run this script to execute all the demo steps one by one. The script stops/breaks after each important step: continue execution by pressing `ENTER`.

At certain stages of the demo script, kafka topics are consumed. The consumer process keeps listening for new records - stop the consumer by hitting `CTRL+C` once you inspected the records in the terminal in order to proceed with the following demo steps.
