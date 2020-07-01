# How to Start Troubleshooting CrashLoopBackoff Errors in Kubernetes Using a Blocking Command

Notice how [this deployment](./deployment.yaml) uses the `sleep infinity` command. This will allow you to bypass the image's default command that is crashing and begin troubleshooting in a terminal.

Use this command to access the pod's terminal:

```bash
kubectl exec -it deploy/wildfly-test -n test-ns -- /bin/bash
```

Read more at: https://austindewey.com/2020/06/30/how-to-start-troubleshooting-crashloopbackoff-errors-in-kubernetes-using-a-blocking-command/