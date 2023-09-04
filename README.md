# ISEC6000-assignment1--task1
#1.1.	Environmental Set Up:

1)	Create an account on the Google cloud platform to access the Kubernetes Engine. In order to use Kubernetes engine, we must register to google cloud platform.
2)	Log in the personal Google cloud account and Created a Project named “ISEC6000”.
3)	Remember to register the payment method before attempting to create a cluster. It is must to have a billable cloud account to access and deploy the cluster privilege.

#1.2.	Creating Kubernetes Cluster on GKE:

After environmental setup, follow the below steps to create a cluster in Kubernetes.
1)	In the ISEC6000 project, navigated inside Kubernetes Engine > Cluster > Enable the API > Create.
   ![image](https://github.com/HariniRavi490/ISEC6000-assignment1--task1/assets/95735756/c3e6e87b-17b7-4f60-9c8f-d162fffe9dab)

3)	Configured the cluster named as isec6000cluster-1 and set the zone as
   ```docker
  	  Australia-southeast2-b
  ```
5)	In next step, configured the default Kubernetes version and node pool with 3 number of nodes.

![image](https://github.com/HariniRavi490/ISEC6000-assignment1--task1/assets/95735756/a46f54c1-843b-40d1-9569-6252a6d0bf46)


 ![image](https://github.com/HariniRavi490/ISEC6000-assignment1--task1/assets/95735756/6e30d6dc-4339-455d-96f6-e9c889cf2e04)

Fig1.2    Configured Kubernetes Version


![image](https://github.com/HariniRavi490/ISEC6000-assignment1--task1/assets/95735756/f900c881-c15c-496f-8719-da25422f8531)

 
Fig:1.3   Configure Node pool



#1.3)    Install and configure Kubernetes:
1.	The Cluster was created in the name of the isec6000-cluster-1 as shown in the Fig 1.4
2.	Google cloud and Kubernetes can be accessed remotely from laptop/Pc with the help of Google cloud shell.
3.	The cloud shell can be activated from cloud console, click on “Activate cloud shell” to access the cloud shell. The cloud shell terminal will prompt in sometime.
  
4.	Connect the Kubernetes Cluster to the local environment.
5.	Set the project with the project ID and configure the zone with below commands.
```ruby
gcloud config set project isec6000-397112
gcloud config set compute/zone australia-southeast2-b

gcloud container clusters get-credentials isec6000-cluster-1 –zone australia-southeast2-b –project isec6000-397112
```

 ![image](https://github.com/HariniRavi490/ISEC6000-assignment1--task1/assets/95735756/340cb0d1-3046-4584-b47b-60ea69784304)

Fig 1.4


