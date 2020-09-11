#topic: Google Cloud Fundamentals: Getting Started with Compute Engine

Objectives
In this lab, you will learn how to perform the following tasks:

Create a Compute Engine virtual machine using the Google Cloud Platform (GCP) Console.

Create a Compute Engine virtual machine using the gcloud command-line interface.

Connect between the two instances.

1.In GCP console, on the top right toolbar, click the Open Cloud Shell button

2. To set your default zone
  <!-- gcloud config set compute/zone  us-central1-b 

  (us-central1-b) being your chosen zone -->


3. To create a VM instance called my-vm-2 in that zone, execute this command:

<!-- gcloud compute instances create "my-vm-2" \
--machine-type "n1-standard-1" \
--image-project "debian-cloud" \
--image "debian-9-stretch-v20190213" \
--subnet "default -->

4. when the vm is lunched type 'exit' in the cloud shell

TOPIC: AK8S-03 Creating a GKE Cluster via GCP Console

Objectives
Use the GCP Console to build and manipulate GKE clusters

Use the GCP Console to deploy a Pod

Use the GCP Console to examine the cluster and Pods

STEPS TO CREATE GRE CLUSTER VIA CLOUD SHELL

1. In the GCP Console, on the Navigation menu click Kubernetes Engine > Clusters.
<!-- 
#In GCP console, on the top right toolbar, click the Open Cloud Shell button -->

<!-- In Cloud Shell, type the following command to set the environment variable for the zone and cluster name. -->

export my_zone=us-central1-a (CHOSE YOUR ZONE)
export my_cluster=standard-cluster-1

TYPE THE FOLLOWING COMMANDS TO CREATE YOUR  GRE CLUSTERS

<!-- gcloud container clusters create $my_cluster --num-nodes 3 --zone $my_zone --enable-ip-alias -->

