# Running Trace-based tests using Tracetest Agent and CLI with Tracetest.io

To add Tracetest to your GitHub pipeline and use [Tracetest CLI](https://docs.tracetest.io/cli/cli-installation-reference) and [Tracetest Agent](https://docs.tracetest.io/concepts/agent) to run tests of [Tracetest.io](https://docs.tracetest.io/), you need just to add the following snippet in your workflow as a step:

```yaml
- name: Configure Tracetest CLI and Agent
  uses: kubeshop/tracetest-github-action@v1
  with:
    token: "{your tracetest token}" # See https://docs.tracetest.io/concepts/environment-tokens for more details
    apiKey: "{your tracetest agent apiKey}" # See https://docs.tracetest.io/concepts/agent for more details
```

You can get your Tracetest Token, on Tracetest.io by following the directions described [here](https://docs.tracetest.io/concepts/environment-tokens). The Tracetest Agent APIKey can be seen on `Agent` tab on `Settings` page.

A full example of usage can be seen on [tracetest-cli-and-agent-with-tracetest-io.yml](./tracetest-cli-and-agent-with-tracetest-io.yml) file located in this folder.
