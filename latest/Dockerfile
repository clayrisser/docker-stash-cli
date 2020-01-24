FROM k8s.gcr.io/hyperkube:v1.12.1

LABEL image=codejamninja/stash-cli \
  maintainer="Jam Risser <jam@codejam.ninja>" \
  base=ubuntu

RUN apt-get update && apt-get install -y \
  wget \
  && rm -rf /var/lib/apt/lists/*
RUN wget -O kubectl-stash \
  https://github.com/stashed/cli/releases/download/v0.3.0/kubectl-stash-linux-amd64 \
  && chmod +x kubectl-stash \
  && mv kubectl-stash /usr/local/bin
