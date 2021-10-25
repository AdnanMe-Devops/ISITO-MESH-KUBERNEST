# ISITO-MESH-KUBERNEST
ISITO TRAFFIC MESH IN KUBERNETES 
Description
Istio is an open source, multi-cloud service mesh, capable of performing intelligent traffic management. Istio's traffic routing rules let you easily control the flow of traffic and API calls to and from deployed cluster resources.

In this Project scenario, w'll learn how to use Istio to perform traffic routing to a pair of sample web applications, V1 and V2, deployed into a Kubernetes cluster and'll then but first setup a traffic routing policy to balance traffic evenly (50/50) across both versions. You'll test and confirm that the traffic is indeed evenly split before later updating the traffic routing policy to use a 80/20 split.

 Objectives
Upon completion of this Lab, you will be able to:

Use Istio to perform traffic routing across a pair of versioned sample web applications 
Configure and deploy the following Istio custom resources:
DestinationRule - the baseline deployment version of the webapp
Gateway - uses a Kustomize overlay to change the baseline deployment settings
VirtualService - uses a Kustomize overlay to change the baseline deployment settings
Test, report, and validate the Istio service mesh based traffic routing using the curl command and your workstations browser

2 x EC2 instances - each assigned a public IP address:
EC2 - provides a web-based IDE with integrated terminal
2EC2 - provides a fully functional and running Kubernetes cluster

Using your local workstation browser to remotely connect to the ide.cloudacademy.platform.instance
Using the web-based IDE and integrated terminal, you'll complete the remainder of the stated Lab Objectives (above)
Deploy V1 and V2 Web Applications

Deploy and Test 50/50 Traffic Routing Policy
 Step, 'll first examine and understand each of the 3 declared Istio custom resources that are used to setup traffic routing to both the V1 and V2 versions of the sample web application. and w'll then use the kubectl command to deploy each of the Istio custom resources into the provided Kubernetes cluster. Finally,  will test and confirm that the applied Istio traffic routing configuration results in traffic routing which is approximately balanced (50/50) across both the V1 and V2 versions of the sample web application.

 Deploy and Test 80/20 Traffic Routing Policy
in this  Step, 'll update the previously deployed traffic routing policy so that it distributes traffic 80% to V1 and 20% to V2. With this in place, w'll again test and confirm that the applied Istio traffic routing configuration results in traffic being approximately balanced (80/20) across the V1 and V2 versions of the sample web application.
