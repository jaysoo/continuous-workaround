This repo shows how to turn off continuous behavior of serve/dev/preview task, and remove it as a dependency of e2e task.

See:
- [main/apps/frontend/project.json](https://github.com/jaysoo/continuous-workaround/blob/main/apps/frontend/project.json) - disables continuous for dev and preview tasks
- [main/apps/frontend-e2e/project.json](https://github.com/jaysoo/continuous-workaround/blob/main/apps/frontend-e2e/project.json) - removes dependencies for e2e task


Running this will kill all processes correctly on Windows.

```shell
nx e2e frontend
```

This is an issue on Windows only, and originally reported here: https://github.com/nrwl/nx/issues/31235

