# prefect-fivetran

## Welcome!

Prefect integrations with Fivetran

## Getting Started

### Python setup

Requires an installation of Python 3.7+.

We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.

These tasks are designed to work with Prefect 2.0. For more information about how to use Prefect, please refer to the [Prefect documentation](https://orion-docs.prefect.io/).

### Installation

Install `prefect-fivetran` with `pip`:

```bash
pip install prefect-fivetran
```

### Write and run a flow

```python
from prefect import flow
from prefect_fivetran.tasks import (
    goodbye_prefect_fivetran,
    hello_prefect_fivetran,
)


@flow
def example_flow():
    hello_prefect_fivetran
    goodbye_prefect_fivetran

example_flow()
```

## Resources

If you encounter any bugs while using `prefect-fivetran`, feel free to open an issue in the [prefect-fivetran](https://github.com/pubchimps/prefect-fivetran) repository.

If you have any questions or issues while using `prefect-fivetran`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack).

## Development

If you'd like to install a version of `prefect-fivetran` for development, clone the repository and perform an editable install with `pip`:

```bash
git clone https://github.com/pubchimps/prefect-fivetran.git

cd prefect-fivetran/

pip install -e ".[dev]"

# Install linting pre-commit hooks
pre-commit install
```
