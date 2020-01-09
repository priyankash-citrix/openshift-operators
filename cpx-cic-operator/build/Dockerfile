FROM quay.io/operator-framework/helm-operator:v0.13.0

### Required OpenShift Labels
LABEL name="Citrix ADC CPX with Citrix Ingress Controller Operator" \
      vendor="Citrix" \
      version="v130.47.102" \
      release="1" \
      summary="This is an helm operator for Citrix ADC CPX with Citrix ingress controller" \
      description="This operator will deploy Citrix ADC CPX with Citrix ingress controller running as side-car in the cluster."

# Required Licenses
COPY licenses /licenses

COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts/ ${HOME}/helm-charts/
