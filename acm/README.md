# ACM Configs for pytest-calculator

## Requirements 
**Confirm target clusters are properly labeled**
> the local-cluster does not need to be checked
*  `clusterid=cluster1`
*  `clusterid=cluster2`
*  `clusterid=cluster3`
*  `clusterid=...`

## pytest development deployment 

**Create namespace for dev environment**
```
oc create -f acm/01_pytest_dev_namespace.yaml
```

**Create Channel for dev environment**
```
oc create -f acm/02_pytest_dev_channel.yaml 
```

**Create Application for dev environment**
```
oc create -f acm/03_pytest_dev_application.yaml
```

### Deploy to pytest-dev local-cluster (ACM HUB)
![20210921225544](https://i.imgur.com/30qHilc.png)
**Deploy pytest-calculator dev environment to local cluster**

**Create Placement rule for local cluster**
```
oc create -f acm/04_pytest_dev_placement_local_cluster.yaml 
```

**Create subscription rule for local cluster**
```
oc create -f acm/05_pytest_dev_subscription_local_cluster.yaml 
```

### Deploy pytest-dev  to cluster1 

**Deploy pytest-calculator dev environment to cluster1**

**Create Placement rule for cluster1**
```
oc create -f acm/04_pytest_dev_placement_cluster1.yaml
```

**Create subscription rule for cluster1**
```
oc create -f acm/05_pytest_dev_subscription_cluster1.yaml
```

### Deploy pytest-dev  to cluster2 

**Deploy pytest-calculator dev environment to cluster2**

**Create Placement rule for cluster2**
```
oc create -f acm/04_pytest_dev_placement_cluster2.yaml
```

**Create subscription rule for cluster2**
```
oc create -f acm/05_pytest_dev_subscription_cluster2.yaml
```


### Deploy pytest-dev  to cluster3 

**Deploy pytest-calculator dev environment to cluster3**

**Create Placement rule for cluster3**
```
oc create -f acm/04_pytest_dev_placement_cluster3.yaml
```

**Create subscription rule for cluster3**
```
oc create -f acm/05_pytest_dev_subscription_cluster3.yaml
```


## pytest production deployment 
![20210921225514](https://i.imgur.com/DxHKVyD.png)
**Create namespace for prod environment**
```
oc create -f acm/01_pytest_prod_namespace.yaml
```

**Create Channel for prod environment**
```
oc create -f acm/02_pytest_prod_channel.yaml 
```

**Create Application for prod environment**
```
oc create -f acm/03_pytest_prod_application.yaml
```

### Deploy to local-cluster (ACM HUB)
**Deploy pytest-calculator prod environment to local cluster**

**Create Placement rule for local cluster**
```
oc create -f acm/04_pytest_prod_placement_local_cluster.yaml 
```

**Create subscription rule for local cluster**
```
oc create -f acm/05_pytest_prod_subscription_local_cluster.yaml 
```

### Deploy pytest-prod  to cluster1 

**Deploy pytest-calculator prod environment to cluster1**

**Create Placement rule for cluster1**
```
oc create -f acm/04_pytest_prod_placement_cluster1.yaml
```

**Create subscription rule for cluster1**
```
oc create -f acm/05_pytest_prod_subscription_cluster1.yaml
```

### Deploy pytest-prod  to cluster2 

**Deploy pytest-calculator prod environment to cluster2**

**Create Placement rule for cluster2**
```
oc create -f acm/04_pytest_prod_placement_cluster2.yaml
```

**Create subscription rule for cluster2**
```
oc create -f acm/05_pytest_prod_subscription_cluster2.yaml
```

### Deploy pytest-prod  to cluster3 

**Deploy pytest-calculator prod environment to cluster3**

**Create Placement rule for cluster3**
```
oc create -f acm/04_pytest_prod_placement_cluster3.yaml
```

**Create subscription rule for cluster3**
```
oc create -f acm/05_pytest_prod_subscription_cluster3.yaml
```