Configuration to install OKD panell in k8s

kubectl apply -f 01_okd.yml

helm repo add av1o https://av1o.gitlab.io/charts

helm -n console upgrade --install okd-console av1o/openshift-console -f values.yaml

kubectl apply -f 02_okd.yml
