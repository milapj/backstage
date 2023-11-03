print("Hello from Tilt")

docker_build('ghcr.io/milapj/backstage/backstage', '.', dockerfile='packages/backend/Dockerfile')

k8s_yaml (
  helm(
    'charts/',
    set=['app.srcFrom=null']
    )
)

k8s_resource('chart-backstage', port_forwards="7007:7007")