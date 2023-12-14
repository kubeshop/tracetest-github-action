# Running Trace-based tests using Tracetest CLI and Tracetest Core

To add Tracetest to your GitHub pipeline and use [Tracetest CLI](https://docs.tracetest.io/cli/cli-installation-reference) to run tests of your own [Tracetest Core server](https://docs.tracetest.io/core/getting-started/installation#install-the-tracetest-server), you need just to add the following snippet in your workflow as a step:

```yaml
- name: Configure Tracetest CLI
  uses: kubeshop/tracetest-github-action@v1
  with:
    endpoint: "{URL to your Tracetest Core Server}"
```

The `endpoint` parameter is the base address where your Tracetest Core Server is installed.

A full example of usage can be seen on [tracetest-cli-with-tracetest-core.yml](./tracetest-cli-with-tracetest-core.yml) file located in this folder.
