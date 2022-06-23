# Copier Terraform Module

This project is a copier template for creating Terraform projects and modules.

The copier template provided here is used to stamp out the GitHub repository template: [aws-ia/terraform-repo-template](https://github.com/aws-ia/terraform-repo-template).

## Prerequisites

This project template uses the [`copier`](https://github.com/copier-org/copier) framework to facilitate project generation.
Copier is a Python CLI and library for rendering project templates.

In order to use this template (and copier, generally), you must first install Python, `git`, and the `copier` module.

- [Download & Install Python 3.7+](https://www.python.org/downloads/)
- [Download & Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [Install `copier`](https://copier.readthedocs.io/en/stable/#installation) (`pip install copier`)

_Note: Please refer to the official Copier documentation if you encounter difficulty [here](https://copier.readthedocs.io/en/stable/#installation)._

## Usage

This project generation template can be used by first installing the pre-requisites annotated above, followed by direct usage of this repository (depending on intended usecase):

### CLI

```bash
# Directly against GitHub repository using HTTPS
copier "https://github.com/aws-ia/copier-terraform-repo-template.git" target/project/path

# or directly against GitHub using the gh shortcut
copier "gh:aws-ia/copier-terraform-repo-template" target/project/path
```

### Programmatically (Python)

```python
from copier import run_auto

# Create a project from this upstream GitHub repository
run_auto("https://github.com/aws-ia/copier-terraform-repo-template.git", "target/project/pathn")

# You can also use "gh:" as a shortcut of "https://github.com/"
run_auto("gh:aws-ia/copier-terraform-repo-template", "target/project/path")
```

_Note: Please refer to the official Copier documentation for further information on using `copier` either programmatically or via the CLI [here](https://copier.readthedocs.io/en/stable/#quick-start)._
