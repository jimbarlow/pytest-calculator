# ACM Configs for pytest-calculator


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
**Deploy pytest-calculator dev environment to local cluster**
![20210921154114](https://i.imgur.com/q0cloJF.png)
**Create Placement rule for local cluster**
```
oc create -f acm/04_pytest_dev_placement_local_cluster.yaml 
```

**Create subscription rule for local cluster**
``
oc create -f acm/05_pytest_dev_subscription_local_cluster.yaml 
``