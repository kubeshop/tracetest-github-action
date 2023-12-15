# Running Trace-based tests using Tracetest CLI with custom config on Tracetest.io

To add Tracetest to your GitHub pipeline and use [Tracetest CLI](https://docs.tracetest.io/cli/cli-installation-reference) to run tests on [Tracetest](https://app.tracetest.io/) using a customized config, you need to add the following snippet in your workflow as a step:

```yaml
- name: Configure Tracetest CLI
  uses: kubeshop/tracetest-github-action@v1
  with:
    configFile: "scheme: https\nendpoint: your.tracetest.url"
```

Where the `configFile` parameter is the content of your CLI config file, usually located in `~/.tracetest/config.yml`.

Here's a full example of how to use it: [tracetest-cli-using-custom-config.yml](./tracetest-cli-using-custom-config.yml)
