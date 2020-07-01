# Helm Tricks: Input Validation with `values.schema.json`

Run this command to render locally:

```bash
helm template validation-test .
```

You'll see the following error:

```
$ helm template validation-test test-chart
Error: values don't meet the specifications of the schema(s) in the following chart(s):
test-chart:
- (root): image is required
- (root): serviceType is required
- (root): port is required
```

The rest of [the post](https://austindewey.com/2020/06/13/helm-tricks-input-validation-with-values-schema-json/) goes into greater detail with how you can see your values being validated against the [values.schema.json](./values.schema.json) file.