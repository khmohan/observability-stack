# 🌟 Observability Stack - Atlan Challenge 2025 🚀  

**A Kubernetes-based observability solution using Prometheus, Grafana, Loki, OpenTelemetry, and Alertmanager.**  

## 📌 Overview  
Welcome to the **Observability Stack** for the **Atlan Challenge 2025!** This repository provides a **comprehensive monitoring solution** for tracking API performance, logs, and traces in real time.  

✅ **Key Benefits:**  
✔️ **Real-time monitoring** with Prometheus  
✔️ **Powerful dashboards** using Grafana  
✔️ **Centralized log aggregation** via Loki  
✔️ **Distributed tracing** using OpenTelemetry  
✔️ **Alerting system** with Alertmanager  
🔧 **Fully containerized & deployed on Kubernetes!**  

## 🚀 Features  
📊 **Metrics Collection** - Prometheus collects real-time system & application metrics.  
🖥️ **Grafana Dashboards** - Pre-built dashboards for easy visualization of logs and metrics.  
🛡️ **Loki Log Aggregation** - Centralized log collection across microservices.  
🔗 **OpenTelemetry Tracing** - Distributed tracing for debugging performance issues.  
⚙️ **Kubernetes-Based Deployment** - Easily deployable on a Kubernetes cluster.  
🚨 **Alertmanager Notifications** - Get alerts for critical system failures.  

## ⚡ Quick Start Guide  
Clone the Repository  
```bash
git clone https://github.com/khmohan/observability-stack.git
cd observability-stack
Deploy the Observability Stack

bash
Copy
Edit
kubectl apply -f manifests/
This deploys Prometheus, Grafana, Loki, OpenTelemetry, and Alertmanager inside the monitoring namespace.

Access Prometheus (Metrics Collection)

bash
Copy
Edit
kubectl port-forward svc/prometheus 9090:9090 -n monitoring
🔗 Open http://localhost:9090 in your browser.

Access Grafana (Visual Dashboards)

bash
Copy
Edit
kubectl port-forward svc/grafana 3000:3000 -n monitoring
🔗 Open http://localhost:3000

Default Login Credentials:

Username: admin

Password: admin (or check the Kubernetes Secret)

View Logs in Loki

bash
Copy
Edit
kubectl port-forward svc/loki 3100:3100 -n monitoring
🔍 Query logs directly in Grafana after adding Loki as a data source.

Monitor Traces with OpenTelemetry

bash
Copy
Edit
kubectl port-forward svc/opentelemetry 4317:4317 -n monitoring
🔗 Configure your applications to send traces to the OpenTelemetry Collector.

Check Alerts in Alertmanager

bash
Copy
Edit
kubectl port-forward svc/alertmanager 9093:9093 -n monitoring
🔗 Open http://localhost:9093 to check active alerts.

📜 Project Structure
graphql
Copy
Edit
📂 observability-stack/
├── 📂 manifests/          # Kubernetes YAML manifests for deployment
├── 📂 dashboards/         # Grafana JSON dashboard configurations
├── 📂 configs/            # Configuration files for Prometheus, Loki, Alertmanager
├── 📄 README.md           # Project documentation
└── 📄 LICENSE             # License details
📌 High-Level System Diagram

(Replace path/to/high-level-diagram.png with the actual path in your repo.)

💪 Contributions & Improvements
🚀 Contributions are welcome! If you find any issues or have ideas to enhance this observability stack, fork the repository and submit a pull request.

📚 Documentation & Resources
📖 Prometheus Docs
📖 Grafana Docs
📖 Loki Docs
📖 OpenTelemetry Docs
📖 Kubernetes Docs








