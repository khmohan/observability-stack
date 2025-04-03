🌟 Observability Stack - Atlan Challenge 2025 🚀

📝 About the Project:

Welcome to the Observability Stack for the Atlan Challenge 2025! This repository provides a comprehensive Kubernetes-based monitoring solution built using Prometheus, Grafana, Loki, and OpenTelemetry. It enables real-time metrics collection, logging, and tracing for your API infrastructure.

🚀 Deploy and monitor your applications seamlessly!

🔧 Features:

🔍 Prometheus for Metrics: Collect real-time system and application metrics.

📊 Grafana Dashboards: Pre-built dashboards for easy visualization.

🛡️ Loki for Log Aggregation: Centralized logging for your microservices.

📲 OpenTelemetry for Tracing: Distributed tracing across services.

⚙️ Kubernetes-Based Deployment: Fully containerized monitoring stack.

🚨 Alertmanager for Notifications: Get alerts for critical issues.

🚀 Quick Start Guide:

1⃣ Clone the Repository

git clone https://github.com/khmohan/observability-stack.git
cd observability-stack

2⃣ Deploy the Observability Stack

Apply the necessary Kubernetes manifests to set up the stack:

kubectl apply -f manifests/

This deploys Prometheus, Grafana, Loki, OpenTelemetry, and Alertmanager inside the monitoring namespace.

3⃣ Access the Prometheus Dashboard

kubectl port-forward svc/prometheus 9090:9090 -n monitoring

Then, open http://localhost:9090 in your browser to explore Prometheus metrics.

4⃣ Access the Grafana Dashboard

kubectl port-forward svc/grafana 3000:3000 -n monitoring

Then, visit http://localhost:3000.

Default Login Credentials:

Username: admin

Password: admin (or check the Kubernetes Secret)

5⃣ View Logs in Loki

kubectl port-forward svc/loki 3100:3100 -n monitoring

Logs can be queried from Grafana by adding Loki as a data source.

6⃣ Monitor Traces with OpenTelemetry

kubectl port-forward svc/opentelemetry 4317:4317 -n monitoring

Configure your applications to send traces to OpenTelemetry Collector.

7⃣ Check Alerts in Alertmanager

kubectl port-forward svc/alertmanager 9093:9093 -n monitoring

Open http://localhost:9093 to check active alerts.

💪 Contributions & Improvements

We welcome contributions! If you find issues or want to enhance the observability stack, fork the repository and submit a pull request.

📜 Documentation & Resources:

Prometheus Docs

Grafana Docs

Loki Docs

OpenTelemetry Docs

Kubernetes Docs

Stay ahead with real-time monitoring and proactive alerting! ✨
