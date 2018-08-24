<!-- Thanks for filing an issue! Before hitting the button, please answer these questions.-->

## Is this a BUG REPORT or FEATURE REQUEST?

restoration backup not working 
apiVersion: mysql.oracle.com/v1alpha1
kind: Restore
metadata:
  name: mysql-restore
spec:
  clusterRef:
     name: mysql-cluster
  backupRef:
     name: mysql-backup
     
     
     <!--
If this is a BUG REPORT, please:
  - Fill in as much of the template below as you can.  If you leave out information, we can't help you as well.

If this is a FEATURE REQUEST, please:
  - Describe *in detail* the feature/behaviour/change you'd like to see.

If we can't reproduce a bug or think a feature already exists, we
might close your issue.  If we're wrong, PLEASE feel free to reopen it and
explain why.
-->

## Versions

**MySQL Operator Version**:

**Environment**:
- **Kubernetes version** (use `kubectl version`): 1.11
- **Cloud provider or hardware configuration**: GCP
- **OS** (e.g. from /etc/os-release):
- **Kernel** (e.g. `uname -a`):  4.15.0-32-generic
- **Others**:

## What happened?
 Warning  FailedValidation  14m   operator-restore-controller  [spec.cluster.name: Required value: a cluster to restore into is required, spec.backup.name: Required value: a backup to restore is required]


## What you expected to happen?
Should successfull restore in the cluster 

## How to reproduce it (as minimally and precisely as possible)?

## Anything else we need to know?
