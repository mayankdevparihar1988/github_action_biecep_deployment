# github_action_biecep_deployment
Sample for github action deployment

# Creating RBAC

* Creating RBAC Crediential 

```bash
 az ad sp create-for-rbac --name "github-az-bicep-spn" \
                         --role contributor \
                         --scopes /subscriptions/0ec3119b-cded-4f46-9ee6-73b60kkkkka/resourceGroups/bicep-dev-eus-rg
```

* Create RBAC WITHOUT ROLE ASSIGNEMET

```bash 
az ad sp create-for-rbac
```

* az role assignment create

```bash 
az role assignment create --assignee $appId  --role contributor

```

```bash 
az ad sp create-for-rbac -n my-biecp-credintial --role Contributor --scopes /subscriptions/0ec3119b-cded-4f46-9ee6-73b601kkkkba/resourceGroups/bicep-dev-eus-rg --sdk-auth
```