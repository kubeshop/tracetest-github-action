# Running Trace-based tests using Tracetest CLI with Tracetest.io

To add Tracetest to your GitHub pipeline and use [Tracetest CLI](https://docs.tracetest.io/cli/cli-installation-reference) to run tests of [Tracetest.io](https://docs.tracetest.io/), you need just to add the following snippet in your workflow as a step:

```yaml
- name: Configure Tracetest CLI
  uses: kubeshop/tracetest-github-action@v1
  with:
    token: "{your tracetest token}" # See https://docs.tracetest.io/concepts/environment-tokens for more details
```

You can get your Tracetest Token, on Tracetest.io by following the directions described [here](https://docs.tracetest.io/concepts/environment-tokens). 

A full example of usage can be seen on [tracetest-cli-with-tracetest-io.yml](./tracetest-cli-with-tracetest-io.yml) file located in this folder.
