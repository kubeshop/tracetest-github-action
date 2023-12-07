# kubeshop/tracetest-github-action

> [GitHub Action](https://docs.github.com/en/actions) for running [Tracetest Agent](https://docs.tracetest.io/getting-started/installation#install-the-tracetest-agent) and/or [Tracetest CLI](https://docs.tracetest.io/getting-started/open#trigger-1) to run trace-based tests against [Tracetest](https://tracetest.io/).

Placing `use: kubeshop/tracetest-github-action@v1` into a GitHub Action workflow gives you a simple way to run Tracetest CLI and/or Tracetest Agent by installing and configuring the tools.

You then proceed to run Tracetest trace-based tests.

You can run this action in four different ways, as seen on [examples](./examples/) folder:

- [Running Trace-based tests using Tracetest Agent and CLI with Tracetest.io](./examples/tracetest-cli-and-agent-with-tracetest-io/)
- [Running Trace-based tests using Tracetest CLI and Tracetest Core](./examples/tracetest-cli-with-tracetest-core/)
- [Running Trace-based tests using Tracetest CLI with Tracetest.io](./examples/tracetest-cli-with-tracetest-io/)
- [Running Trace-based tests using Tracetest CLI with custom config on Tracetest.io](./examples/tracetest-cli-using-custom-config/)
