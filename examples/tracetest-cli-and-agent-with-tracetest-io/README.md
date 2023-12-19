# Running Trace-based Tests using Tracetest Agent and CLI with Tracetest.io

To add Tracetest to your GitHub pipeline and use [Tracetest CLI](https://docs.tracetest.io/cli/cli-installation-reference) and [Tracetest Agent](https://docs.tracetest.io/concepts/agent) to run tests on [Tracetest](https://app.tracetest.io/), you need to add the following snippet in your workflow as a step:

```yaml
- name: Configure Tracetest CLI and Agent
  uses: kubeshop/tracetest-github-action@v1
  with:
    token: "{your tracetest token}" # See https://docs.tracetest.io/concepts/environment-tokens for more details
    apiKey: "{your tracetest agent apiKey}" # See https://docs.tracetest.io/concepts/agent for more details
```

You can get your Tracetest Token from the Tracetest settings page by following the directions described [here](https://docs.tracetest.io/concepts/environment-tokens). The Tracetest Agent APIKey can be seen on the `Agent` tab on `Settings` page.

If you don't need to start an Agent on your GitHub pipeline, you can declare only the `token` parameter and use it. You can see more details on [Running Trace-based Tests using Tracetest CLI with Tracetest.io
](https://github.com/kubeshop/tracetest-github-action/tree/main/examples/tracetest-cli-with-tracetest-io).

Here's a full example of how to use it: [tracetest-cli-and-agent-with-tracetest-io.yml](./tracetest-cli-and-agent-with-tracetest-io.yml) 
