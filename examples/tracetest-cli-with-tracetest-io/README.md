# Running Trace-based Tests using Tracetest CLI with Tracetest.io

To add Tracetest to your GitHub pipeline and use [Tracetest CLI](https://docs.tracetest.io/cli/cli-installation-reference) to run tests on [Tracetest](https://app.tracetest.io/), you need to add the following snippet in your workflow as a step:

```yaml
- name: Configure Tracetest CLI
  uses: kubeshop/tracetest-github-action@v1
  with:
    token: "{your tracetest token}" # See https://docs.tracetest.io/concepts/environment-tokens for more details
```

You can get your Tracetest Token on the Tracetest settings page by following the directions described [here](https://docs.tracetest.io/concepts/environment-tokens). 

Here's a full example of how to use it: [tracetest-cli-with-tracetest-io.yml](./tracetest-cli-with-tracetest-io.yml)
