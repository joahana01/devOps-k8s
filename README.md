**Autor:** Johana Rangel Albarran

# DevOps K8s - Manifiestos Kubernetes

Manifiestos para desplegar `joahanagit/devops-test` en Kubernetes.

# Clonar el repositorio
git clone https://github.com/joahana01/devOps-test.git
cd devOps-test

## Desplegar

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml


#Probar con la IP externa
curl http://[EXTERNAL-IP]/health

#Monitoreo basico

# Ver logs del pod
kubectl logs -f deployment/devops-test

# Ver estado de los pods
kubectl get pods -w
