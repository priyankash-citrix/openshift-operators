# Build the manager binary
FROM quay.io/operator-framework/helm-operator:v1.28.1
LABEL name="Citrix Ingress Controller Operator" \
      vendor="Citrix" \
      version="v1.33.4 " \
      release="1" \
      summary="This is an Citrix Ingress Controller helm operator." \
      description="This operator will deploy Citrix Ingress Controller to the cluster."

COPY licenses /licenses
ENV HOME=/opt/helm
COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts  ${HOME}/helm-charts
WORKDIR ${HOME}
