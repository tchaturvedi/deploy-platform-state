# deploy-platform-state

GitOps state repo for [deploy-platform](https://github.com/tchaturvedi/deploy-platform) — see
`deploy-platform/docs/design.md` §6 for the layout rationale and `docs/adr/0010-gitops-repo-split.md`
for why this is a separate repo from platform source.

ArgoCD is the only writer that applies anything from here to the cluster; commits land here either
via the deploy-platform API (once built) or, for now, manually while that API doesn't exist yet.
