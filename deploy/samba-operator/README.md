# Samba Operator HELM chart

## Overview

Chart that installs Samba Operator and CRDs. CRDs are applied only when doing the initial install. Any further updates to CRDs need to be applied manually.

## Packaging

```sh
helm package .
helm push samba-operator-0.1.0.tgz oci://repository
```

## Usage

```sh
helm install -n <namespace> . --create-namespace --wait
```