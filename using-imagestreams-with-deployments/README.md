Be sure to create a pull secret before creating the ImageStream.

```bash
oc create secret docker-registry redhat-auth --docker-server=registry.redhat.io --docker-username=$USERNAME --docker-password=$PASSWORD --docker-email=unused
```
