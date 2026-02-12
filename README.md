# GKE Multi-Cluster Config Sync Repository

## Structure
- clusters/ → per-cluster configuration
- shared/ → global reusable configs
- system/ → RootSync templates

## Setup

1. Enable Config Sync
2. Apply RootSync:

kubectl apply -f system/rootsync-template.yaml

3. Verify:

kubectl -n config-management-system get rootsync
