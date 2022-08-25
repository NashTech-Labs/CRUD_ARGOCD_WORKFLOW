# CRUD_ARGOCD_WORKFLOW

## Argocd
Argo CD is a declarative, GitOps continuous delivery tool for Kubernetes. 

## Argocd Python Client

For Install Argocd Python Client using following command:

```
$ pip install argo-workflows
```

## CRUD Workflow using Argocd Python Client:
For creating, listing , updating and deleting workflows using this python client we need to give our configurations in crud_workflow.py file:

```
configuration = argo_workflows.Configuration(host="<YOUR_ARGOCD_SERVER_ENDPOINT>")

```

And you have to give the name and namespace of that workflow which you want to delete:

```
namespace = "<NAMESPACE_OF_ARGOWORKFLOW>"
name= "<NAME_OF_WORKFLOW"
```

```
namespace = "argo"  
name= "hello-yami-8q2kc"
```


## Run the python file:

```
$ python3 crud_workflow.py
```

Uncomment the specific create_workflow , list_workflows, update_workflow and delete_workflow as per operation

## NOTE
```
Use the Bearer Token in case of need
```