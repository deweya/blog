# Method #2 - Environment Variables

Build with this command:

```bash
docker build -t scl-test:latest .
docker run --name scl-test -it scl-test /bin/bash -c "python --version"
```

The result should be similar to:

```
Python 3.5.1
```