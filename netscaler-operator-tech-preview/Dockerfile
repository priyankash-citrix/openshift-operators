# Build the manager binary
FROM quay.io/operator-framework/helm-operator:v1.30.0

LABEL name="NetScaler Operator" \
      vendor="NetScaler" \
      version="1.1.0" \
      release="1" \
      summary="This is an operator to install cloud native portfolio provided by Netscaler" \
      description="This is an operator to install cloud native portfolio provided by Netscaler"

COPY licenses /licenses
ENV HOME=/opt/helm
COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts  ${HOME}/helm-charts
WORKDIR ${HOME}
