# kubectl strip-cm

![kubectl-strip-cm.gif](https://github.com/SoulChildTc/kubectl-strip-cm/raw/main/kubectl-strip-cm.gif?raw=true)

## Installation

```bash
curl -LO https://github.com/SoulChildTc/kubectl-strip-cm/raw/main/kubectl-strip_cm
chmod +x ./kubectl-strip_cm
sudo mv ./kubectl-strip_cm /usr/local/bin/kubectl-strip_cm
```

## Usage

```bash
# Purify your configmap
k strip-cm -n kube-system filebeat-config

# use the -f option, ignore prompts.
k strip-cm -n kube-system filebeat-config -f
```


k edit cm -n kube-system filebeat-config
k strip-cm -n kube-system filebeat-config