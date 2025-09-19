# https://git
kustomize.io/

# https://kubernetes.io/docs/tasks/manage-kubernetes-objects/kustomization/






https://kubectl.docs.kubernetes.io/references/kustomize/kustomization/patches/





# erstelle ein secret und sofort mit einem pub key selean
k -n kafka create secret generic extern.user1 \
  --from-literal=password=supersecret \
  --dry-run=client -o yaml | \
kubeseal \
  --cert public-key \
  --format yaml > extern-user1-sealedsecret.yaml
