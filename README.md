# Deploy Riot Matrix Chat Server for SciCat Science Logbook 🧑‍🔬💬  

This repository provides the configuration and setup for deploying a **Riot Matrix chat server** to support the **SciCat Science Logbook**. The chat server is designed for discussing results, sharing insights, and posting visualizations directly from the SciCat Science Catalogue at **ESS (European Spallation Source)**.

---

## Features ✨  

- **Matrix Chat Server**: Real-time communication and collaboration platform.  
- **Riot Web Client**: User-friendly web interface for interacting with the chat.  
- **SciCat Integration**: Post results and visualizations from the SciCat Science Catalogue.  
- **Scalable Deployment**: Configured for Kubernetes with Helm for efficient management.  

---

## Prerequisites 🛠️  

- A running Kubernetes cluster.  
- Helm installed on your system.  
- Kubernetes CLI (`kubectl`) configured.  

---

## Installation  

1. Clone the repository:  
git clone https://github.com/your-username/sci-chat-matrix-server.git  
cd sci-chat-matrix-server  

2. Deploy with Helm:  
helm install riot-matrix ./helm-chart  

3. Verify Deployment:  
kubectl get pods  

4. Access the Riot web client:  
Set up an Ingress controller and navigate to the configured URL.  

---

## Configuration  

1. Update the `values.yaml` file in the Helm chart to customize:  
   - Riot web client settings  
   - Matrix server configurations  
   - Ingress domain and paths  

2. Apply Kubernetes resources:  
kubectl apply -f ingress.yaml  

3. Check logs for debugging:  
kubectl logs <pod-name>  

---

## File Structure 📂  

- `helm-chart/`: Helm chart for deploying Riot and Matrix.  
- `kubernetes/`: Additional Kubernetes configurations (e.g., Ingress, Services).  
- `README.md`: Documentation for the repository.  

---

## Example Commands  

- Deploy using Helm:  
  helm install riot-matrix ./helm-chart  

- View running services:  
  kubectl get services  

- Apply Ingress:  
  kubectl apply -f ingress.yaml  

---

## Contributing 🤝  

1. Fork the repository.  
2. Create a new branch:  
git checkout -b feature/your-feature  

3. Commit your changes:  
git commit -m "Add your feature"  

4. Push the branch:  
git push origin feature/your-feature  

5. Open a pull request.  

---

## License 📝  

This project is licensed under the MIT License. See the LICENSE file for details.  

---

**Enhance collaboration with the SciCat science logbook using Riot Matrix chat!** 🧑‍🔬💬  
