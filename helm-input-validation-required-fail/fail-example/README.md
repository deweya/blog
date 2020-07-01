# fail-example

Run with the following command:

```bash
helm template fail-test . --values values.yaml
```

You should see the following output:

```
Error: template: fail-example/templates/configmap.yaml:10:4: executing "fail-example/templates/configmap.yaml" at <fail "Invalid function type">: error calling fail: Invalid function type

Use --debug flag to render out invalid YAML
```