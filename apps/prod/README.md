# prod

Production Argo CD applications can be added here once production manifests or Helm values are ready.

Rules for prod:

- Do not enable `spec.syncPolicy.automated` for prod applications.
- Promote to prod only from `main`.
- Keep GitHub Actions prod workflows manual with `workflow_dispatch`.
- Protect the GitHub `prod` environment with required reviewers.
