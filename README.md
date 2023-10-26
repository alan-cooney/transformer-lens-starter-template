# Transformer Lens Starter Template

A simple starter template to get going with Transformer Lens.

## Getting Started

1. Click "Use this template" from GitHub, to create your new repo.

   [![Static
   Badge](https://img.shields.io/badge/Use%20the%20template-rgb(31%2C%20136%2C%2061)?style=for-the-badge&logo=github)
   ](https://github.com/new?template_name=transformer-lens-starter-template&template_owner=alan-cooney)

2. Follow the steps below, depending on what system you're using.

### System Setup

#### Mac (apple silicon)

Apple silicon doesn't play well with Docker, so instead we'll use the poetry virtual environment
(i.e. don't click yes if VSCode asks if you want to open your project in a devcontainer).

However, this means you'll need to install some dependencies:

1. Install Brew if you don't have it (package manager a bit like apt)

    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

2. Install some dependencies:

   ```bash
   brew install python@3.9 python@3.10 python@3.11 node poetry pip virtualenv
   ```

3. Install [VSCode](https://code.visualstudio.com/) if you don't have it already
4. Clone your newly created repo onto your local system.
5. Open the folder in VSCode and select "no" to opening the devcontainer with Docker.
6. Install the dependencies with [Poetry](https://github.com/python-poetry/poetry), or pip.

   ```bash
   poetry config virtualenvs.in-project true # [Optional] Default to creating .venv in project dir
   poetry install # Install
   poetry env use python3.11 # [Optional] use a specific python version
   ```

   ```bash
   pip install .
   ```

7. In VSCode set your default interpretor to the virtual environment (`CMD+SHIFT+P` then `>Python:
   Select Interpretor`. Choose the one in the virtual environment ('.venv: Poetry'). Then reload the
   window (`CMD+SHIFT+P` then `>Developer: Reload Window`).

#### Windows/Linux (local only)

1. Install the following:

   - [VSCode](https://code.visualstudio.com/)
   - [Remote Development VSCode
     Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)
   - [Docker for Windows](https://docs.docker.com/desktop/install/windows-install/)

2. Clone your newly created repo onto your local system.
3. Open the folder in VSCode and click "yes" to opening the devcontainer with Docker.
4. In VSCode set your default interpretor to the virtual environment (`CMD+SHIFT+P` then `>Python:
   Select Interpretor`. Choose the one in the virtual environment ('.venv: Poetry'). Then reload the
   window (`CMD+SHIFT+P` then `>Developer: Reload Window`).

#### Remote SSH (e.g. VastAI)

1. Setup any SSH keys needed to connect to your remote (host) box (e.g. [see
   this](https://vast.ai/faq#SSH) with VastAI)
2. Install locally (on your laptop connecting to the box) the following:
   - [VSCode](https://code.visualstudio.com/)
   - [Remote Development VSCode
     Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)
3. Connect to the host box from within VSCode using [these
   instructions](https://code.visualstudio.com/docs/remote/ssh-tutorial#_connect-using-ssh).
4. Clone the repo you've already created (from the template) on this remote box.
5. Open the cloned repo folder with VSCode
6. Click "yes" to opening the devcontainer with Docker.
7. In VSCode set your default interpretor to the virtual environment (`CMD+SHIFT+P` then `>Python:
   Select Interpretor`. Choose the one in the virtual environment ('.venv: Poetry'). Then reload the
   window (`CMD+SHIFT+P` then `>Developer: Reload Window`).

## Troubleshooting

If you have any issues, just open an issue with your question. I'll try to respond as quickly as
possible, and also add the solution to the README.
