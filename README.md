# keycloak-helm

![Lifecycle:Stable](https://img.shields.io/badge/Lifecycle-Stable-97ca00)

repository for keycloak images and helm chart

```
| es sql="select \"@timestamp\", labels.audit_type from hive where container.labels.namespace='6d70e7-test' AND container.name='sso-keycloak'"
| search labels.audit_type != null
| eval time=strftime(_time, "%Y-%m-%d")
| timechart span=1d count by labels.audit_type
```