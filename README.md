# k8s-kong-ingress-secret-tls
k8s-kong-ingress-secret-tls

# k8s-kong-ingress-secret-tls
Tutorial
- Apply ingress kong with SSL Letsencrypt

### 1. Install Kong Gateway (OSS) on Kubernetes native
   ```bash
   kubectl apply -f https://bit.ly/kong-ingress-dbless
   ```
### 2. Clone this project into your workspace
   ```bash
   git clone https://github.com/alendwahida/k8s-kong-ingress-secret-tls.git
   ```
### 3. Generate your certificate file from ssl provider or letsencrypt
### 4. Create secret within ssl certificate into file awn.my.id.crt and key into awn.my.id.key
   ```bash
   kubectl create secret tls awn-tls --key="awn.my.id.key" --cert="awn.my.id.crt"
   ```
### 5. Output:
![alt text](https://raw.githubusercontent.com/alendwahida/k8s-kong-ingress-secret-tls/main/blob/kong-ssl-lets-encrypt.jpg)

### source: https://docs.konghq.com/gateway/2.8.x/install-and-run/kubernetes/
