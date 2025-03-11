## Architecture

### Storage

[Longhorn](https://longhorn.io/) is used as a tool for persistent storage. In case of uninstalling Longhorn from the cluster, deleting all workloads (PersistentVolume, PersistentVolumeClaim, StorageClass, Deployment, StatefulSet, DaemonSet, etc.) using Longhorn volumes is recommended to prevent damage to the cluster.

OCI Object Storage is used as a storage backup solution for the cluster. Detailed setup can be found [here](https://docs.oracle.com/en/learn/object-storage-longhorn-backups/index.html#task-4-create-a-kubernetes-secret).
