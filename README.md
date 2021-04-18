## Network Policy Demo for KCDA 2021

- [Slide Link](https://drive.google.com/file/d/1r_XPXX0abgRED93cezQhb8WJrSwdi8M8/view?usp=sharing)


### Usage
- Deploy resource without network policy
```bash
  $ cp kustomization-without-policy.yaml kustomization.yaml
  $ kustomize build . |kubectl apply -f -
```
Test communication between pods by execing into any pod and try curling or telneting

- Deploy resource with enforced network policy
```bash
  $ cp kustomization-with-policy.yaml kustomization.yaml
  $ kustomize build . |kubectl apply -f -
```
Test communication between pods by execing into any pod and try curling or telneting again.
