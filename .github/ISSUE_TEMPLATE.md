<!-- Thanks for filing an issue! Before hitting the button, please answer these questions.-->

## Is this a BUG REPORT or FEATURE REQUEST?

Choose one: BUG REPORT 

## Versions

**MySQL Operator Version**:

**Environment**:
- **Kubernetes version** (use `kubectl version`): 1.11 
- **Cloud provider or hardware configuration**: GCP
- **OS** (e.g. from /etc/os-release):
- **Kernel** (e.g. `uname -a`): 
- **Others**: 

## What happened?
When excuted the folowing restore file 
apiVersion: mysql.oracle.com/v1alpha1
kind: Restore
metadata:
  name: example-restore
spec:
  clusterRef:
    name: mycluster
  backupRef:
    name: mysql-backup

this error : 
Warning  FailedValidation  14m   operator-restore-controller  [spec.cluster.name: Required value: a cluster to restore into is required, spec.backup.name: Required value: a backup to restore is required]
## What you expected to happen?
Should successfully restore the backup file to the cluster 


## How to reproduce it (as minimally and precisely as possible)?

## Anything else we need to know?
