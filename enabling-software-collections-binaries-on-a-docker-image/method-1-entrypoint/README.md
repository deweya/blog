# Method #1 - Entrypoint

Build with this command:

```bash
docker build -t scl-test:latest .
docker run --name scl-test -it scl-test python --version
```

The output should be similar to:

```
Python 3.5.1
```