# Lab3 and Lab4 Experiment Record

- Student: 姜丞骏
- GitHub account: whatokk
- Experiments:
  - Lab3: Kubernetes and Minikube tutorials
  - Lab4: Istio Getting Started with Bookinfo and dashboard add-ons
- Evidence repository: https://github.com/whatokk/cloud-labs-03-04-kubernetes-istio
- Successful Actions run: https://github.com/whatokk/cloud-labs-03-04-kubernetes-istio/actions/runs/27429016540
- Execution environment: GitHub Actions Ubuntu runner with Docker, minikube, kubectl, and istioctl

## Lab3 Key Results

- Started a minikube Kubernetes cluster with the Docker driver.
- Deployed and exposed `hello-minikube`; HTTP access returned the echo server response.
- Deployed `kubernetes-bootcamp`, inspected pod details, logs, and environment variables.
- Exposed the bootcamp deployment through NodePort and verified HTTP access.
- Scaled the deployment to 4 replicas and observed requests served by multiple pods.
- Performed a rolling update to `nginx:1.27-alpine` and rolled back to `gcr.io/google-samples/kubernetes-bootcamp:v1`.

## Lab4 Key Results

- Installed Istio 1.27.1 with the demo profile.
- Verified `istiod`, ingress gateway, and egress gateway pods in `istio-system`.
- Installed Gateway API CRDs and created the Bookinfo Gateway and HTTPRoute.
- Deployed Bookinfo services and confirmed productpage, details, ratings, and reviews pods were running with sidecars.
- Accessed the Bookinfo Product Page through port-forward; the HTML title was `Simple Bookstore App`.
- Installed dashboard add-ons and verified Kiali, Prometheus, Grafana, tracing, and jaeger-collector services.

## Submitted PDFs

- `reports/whatokk_Lab3_Kubernetes_Minikube_Report.pdf`
- `reports/whatokk_Lab4_Istio_Bookinfo_Report.pdf`
- `reports/whatokk_Lab3_Lab4_Kubernetes_Istio_Report.pdf`
