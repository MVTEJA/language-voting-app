# Steps included in creating this project:

1. **Setup EKS Cluster with NodeGroup:**
    - Create an EKS cluster with a NodeGroup containing 2 nodes of the t2.medium instance type.

2. **IAM Role for EC2:**
    - Create an IAM role for EC2 instances with specific permissions for EKS actions.

3. **Install Kubectl:**
    - Download and install `kubectl`, the Kubernetes command-line tool.

4. **Install AWS CLI:**
    - Download and install the AWS CLI.

5. **Configure Kubectl:**
    - Set the Kubernetes context using `aws eks update-kubeconfig` command.

6. **Clone GitHub Repo:**
    - Clone the GitHub repository containing the Kubernetes manifests.

7. **Create Namespace:**
    - Create a Kubernetes namespace named `cloudchamp`.

8. **Mongo Database Setup:**
    - Apply YAML files for Mongo StatefulSet and Service.
    - Initialize the MongoDB Replica Set.
    - Load initial data into the MongoDB database.

9. **Create Mongo Secret:**
    - Apply a YAML file for creating a secret for MongoDB.

10. **API Setup:**
    - Deploy the GO API using Kubernetes manifests.
    - Expose the API deployment through a LoadBalancer service.

11. **Test API Endpoints:**
    - Test API endpoints `/languages`, `/languages/{name}` to ensure they can be called successfully.

12. **Frontend Setup:**
    - Deploy the Frontend using Kubernetes manifests.
    - Expose the Frontend deployment through a LoadBalancer service.

13. **Test End-to-End Application:**
    - Confirm that the Frontend ELB is ready to receive traffic.
    - Generate the Frontend URL and test the full end-to-end cloud-native application.

14. **Summary:**
      Successfully orchestrated the deployment of a cloud-native web application on Amazon EKS.
      Demonstrated proficiency in setting up an EKS cluster with a NodeGroup, ensuring a scalable and highly available infrastructure.
      
      Implemented MongoDB as the backend database with a ReplicaSet, ensuring data redundancy and high availability.
      Confirmed the successful recording of data within the MongoDB ReplicaSet, highlighting the reliability of the chosen data storage solution.
