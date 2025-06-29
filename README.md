# Info despliegue manual
Para hacer un despliegue manual en tu clúster K3s, no necesitas agregar los pasos de kubectl en el workflow de GitHub Actions. Puedes hacerlo directamente desde tu máquina local o desde el runner si tienes acceso.

1. Pasos para el despliegue manual
Asegúrate de que tu clúster pueda acceder a la imagen
Ya que la imagen está en Docker Hub (mscjaime/my-python-app:latest), tu clúster podrá descargarla.

2. Aplica el manifiesto de Kubernetes manualmente
Ejecuta este comando desde una terminal que tenga acceso al clúster (por ejemplo, tu PC con kubectl configurado):

```bash
kubectl apply -f k8s/deployment.yaml
```

Verifica el despliegue