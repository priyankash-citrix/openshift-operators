# Build the manager binary
FROM quay.io/operator-framework/helm-operator:v1.23.0

### Required OpenShift Labels
LABEL name="Citrix ADC CPX with Citrix Ingress Controller Operator" \
      vendor="Citrix" \
      version="v1.26.7" \
      release="1" \
      summary="This is an Citrix ADC CPX with Citrix ingress controller helm operator." \
      description="This operator will deploy Citrix ADC CPX with Citrix ingress controller running as side-car, in the cluster."

COPY licenses /licenses
ENV HOME=/opt/helm
COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts  ${HOME}/helm-charts
WORKDIR ${HOME}
