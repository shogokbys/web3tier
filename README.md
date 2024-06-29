# web3tier

## Description
web3tier is a project designed to demonstrate the capability of Kubernetes (K8s) container instantiation and load balancing using a simple three-tier web application. This project provides an example of how to set up and manage a multi-tier application on a K8s cluster.

## Installation
To install and deploy web3tier, apply the provided manifest files on any Kubernetes cluster. Ensure that you have a running K8s cluster and `kubectl` configured to interact with it.

1. Clone the repository:
   ```sh
   git clone https://github.com/shogokbys/web3tier.git
   cd web3tier
   ```

2. Apply the Kubernetes manifests:
   ```sh
   kubectl apply -f manifests/
   ```

## Usage
1. Check the front end external IP address of the `frontend` service by using the following command:
   ```sh
   kubectl get svc -n <namespace>
   ```
   Replace `<namespace>` with the appropriate namespace where the services are deployed.

2. Access the external IP address using any web browser. Refresh the page a few times and confirm if the hostname changes each time you access it. This demonstrates the load balancing in action.

## Contributing
Contributions are welcome! Please submit a pull request or open an issue to discuss any changes or improvements.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For any questions or inquiries, please contact [your email] or open an issue on GitHub.