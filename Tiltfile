print("Hello from Tilt")

docker_build('backstage', 'packages/backend/', dockerfile='packages/backend/Dockerfile')

k8s_yaml (
  helm(
    'charts/',
    set=['app.srcFrom=null']
    )
)