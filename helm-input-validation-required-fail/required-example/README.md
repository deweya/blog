# required-example
Run with the following command:

```bash
helm template required-test .
```

You should see the following output:

```
Error: execution error at (required-example/templates/configmap.yaml:4:11): Name of ConfigMap is required

Use --debug flag to render out invalid YAML
```