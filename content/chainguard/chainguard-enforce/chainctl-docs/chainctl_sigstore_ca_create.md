---
date: 2023-01-31T17:36:40-05:00
title: "chainctl sigstore ca create"
slug: chainctl_sigstore_ca_create
url: /chainguard/chainguard-enforce/chainctl-docs/chainctl_sigstore_ca_create/
draft: false
images: []
type: "article"
toc: true
---
## chainctl sigstore ca create

Create a certificate authority instance.

```
chainctl sigstore ca create --group GROUP_NAME | GROUP_ID {--ca googleca --googleca-ref RESOURCE | --ca kmsca --kms-key-ref RESOURCE --kms-cert-chain CERT} [--description DESCRIPTION] [--name NAME] [--output table|json|id] [flags]
```

### Options

```
      --ca string               certificate authority type: [ kmsca | googleca ]
  -d, --description string      The description of the resource.
      --googleca-ref string     CA service resource, in the format /projects/<project>/locations/<location>/<name>
      --group string            The parent group name or id of the sigstore instance.
  -h, --help                    help for create
      --kms-cert-chain string   Path to file containing PEM-encoded root certificate and chain
      --kms-key-ref string      KMS key resource, prefixed with gcpkms://
  -n, --name string             Given name of the resource.
```

### Options inherited from parent commands

```
      --api string                   The url of the Chainguard platform API. (default "http://api.api-system.svc")
      --audience string              The Chainguard token audience to request. (default "http://api.api-system.svc")
      --config string                A specific chainctl config file.
      --console string               The url of the Chainguard platform Console. (default "http://console-ui.api-system.svc")
      --issuer string                The url of the Chainguard STS endpoint. (default "http://issuer.oidc-system.svc")
  -o, --output string                Output format. One of: ["", "table", "tree", "json", "id", "wide"]
      --timestamp-authority string   The url of the Chainguard Timestamp Authority endpoint. (default "http://tsa.timestamp-authority.svc")
```

### SEE ALSO

* [chainctl sigstore ca](/chainguard/chainguard-enforce/chainctl-docs/chainctl_sigstore_ca/)	 - Sigstore commands related to certificate authorities
