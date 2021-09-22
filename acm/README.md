# ACM Configs for pytest-calculator

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

### Deploy to local-cluster (ACM HUB)
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