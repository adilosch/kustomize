# https://git
kustomize.io/

# https://kubernetes.io/docs/tasks/manage-kubernetes-objects/kustomization/






https://kubectl.docs.kubernetes.io/references/kustomize/kustomization/patches/



  authentication:
    type: scram-sha-512
    password:
      valueFrom:
        secretKeyRef:
          name: extern.user1]
          key: password 

