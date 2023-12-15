# Running Trace-based Tests using Tracetest CLI and Tracetest Core

To add Tracetest to your GitHub pipeline and use [Tracetest CLI](https://docs.tracetest.io/cli/cli-installation-reference) to run tests on your own [Tracetest Core Server](https://docs.tracetest.io/core/getting-started/installation#install-the-tracetest-server), you need to add the following snippet in your workflow as a step:

```yaml
- name: Configure Tracetest CLI
  uses: kubeshop/tracetest-github-action@v1
  with:
    endpoint: "{URL to your Tracetest Core Server}"
```

The `endpoint` parameter is the base address where your Tracetest Core Server is installed.

Here's a full example of how to use it: [tracetest-cli-with-tracetest-core.yml](./tracetest-cli-with-tracetest-core.yml)
