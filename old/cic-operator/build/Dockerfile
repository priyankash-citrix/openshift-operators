FROM quay.io/operator-framework/helm-operator:v0.19.3

LABEL name="Citrix Ingress Controller Operator" \
      vendor="Citrix" \
      version="v1.9.2" \
      release="1" \
      summary="This is an CIC helm operator." \
      description="This operator will deploy CIC to the cluster."

COPY licenses /licenses

COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts/ ${HOME}/helm-charts/
