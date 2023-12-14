# Running Trace-based tests using Tracetest CLI with custom config on Tracetest.io

To add Tracetest to your GitHub pipeline and use [Tracetest CLI](https://docs.tracetest.io/cli/cli-installation-reference) to run tests of [Tracetest.io](https://docs.tracetest.io/) using a customized config, you need just to add the following snippet in your workflow as a step:

```yaml
- name: Configure Tracetest CLI
  uses: kubeshop/tracetest-github-action@v1
  with:
    configFile: "scheme: https\nendpoint: your.tracetest.url"
```

Where the `configFile` parameter is the contents of your CLI config file, usually located on `~/.tracetest/config.yml`.

A full example of usage can be seen on [tracetest-cli-using-custom-config.yml](./tracetest-cli-using-custom-config.yml) file located in this folder.
