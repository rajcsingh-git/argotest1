# argotest1

Add following annotations for ingress in metadata

  annotations:
    kubernetes.io/ingress.class: nginx
    nginx.ingress.kubernetes.io/force-ssl-redirect: "true"
    nginx.ingress.kubernetes.io/ssl-passthrough: "true"


Edit deployment ingress-nginx-controller in ingress-nginx namespace in spec.containers.-args

  -- -enable-ssl-passthrough
