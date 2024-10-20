# Fall 2024 Class 05 - More Deep Learning Tools

This class reviews more tools in our machine learning ecosystem, including more advanced PyTorch examples, ONNX, captum, and lightning.

## Installation and Use via Github Codespaces (Recommended for Lightweight Use ONLY!)

To use this repository via codespaces simply click on the `code` &rarr; `codespaces` &rarr; `create codespace on main` buttons.

Once the codespace is open in the browser, click the three bars in the top left corner and select `Open in VS Code Desktop`.

Widgets might work better when using VS Code Desktop vs. in the browser.

Note the codespace might take a long time to build. This is usually due to TexLive dependencies. Use `Cmd` / `Ctrl` + `Shift` + `P` &rarr; `Codespaces: View Creation Logs` to check status.

If required, use `Cmd` / `Ctrl` + `Shift` + `P` &rarr; `Codespaces: Rebuild Container` to rebuild the container. Do not use `gh codespace rebuild`. This takes a long time since it re-downloads the entire image.

**WARNING: This repository contains scripts which can help download large sets of data (10s of GBs) for academic machine learning projects. If you perform these downloads in codespaces, you will risk using up all your free storage for the month!**

## Installation via a Dev Container (Recommended for Development)

If developing on this project, it is recommended to use a locally hosted Dev Container. Codespaces is not recommended since downloading large datasets can consume space (which may be a problem if you want to stay under the free limit for codespaces).

To use this repository via a Dev Container, be sure you have the Dev Containers extension installed, along with Docker Desktop and WSL 2 (Windows only). Clone the repository, open VS Code in the repository root, and click the button shown in the pop up in the bottom-right corner to open in the Dev Container.

If the popup doesn't show type `Cmd` / `Ctrl` + `Shift` + `P` &rarr; `Reopen in Container` (if the container is already built) or `Cmd` / `Ctrl` + `Shift` + `P` &rarr; `Build and Open in Container` if the container is not yet built.

## Usage in a Dev Container

### Using the Python Data Generators via a Devcontainer

@TODO (Mauro Sanchirico): Populate

### Using the NBIA Data Loaders via a Devcontainer

@TODO (Mauro Sanchirico): Populate

### Display of Presentations in a Dev Container

This repository contains some presentations made in reveal.js. To view this, navigate to the `presentations` folder.

```bash
cd presentations
```

Start an http-server.

```bash
bash ../scripts/start_server.sh
```

## Local Installation

The dependencies required for local installation can be found in `.devcontainer/Dockerfile` and `.devcontainer/configure_environment.sh`.

For local installation, perform setup and install dependencies in the order they appear in the Dockerfile and the configuration script, starting with the Dockerfile.

Final setup commands can be found in `.devcontainer/post_attach.sh`.

Note that setup will be different depending on the local OS.

#### Viewing HTML Pages Directly in a Browser from Local Installation

To view HTML pages directly in a browser, simply navigate to the pages of interest and open them with a preferred web browser.

#### Selecting the Correct Python Interpreter

If the correct Python interpreter is not selected by default, select it manually in VS Code.

Open the command pallette with `Ctrl` + `Shift` + `P` and type `Python: Select Interpreter`.

Now specify that VSCode should use the that interpreter (the one in `./.venv/Scripts/python.exe`). Once you specify this, Jupyter notebooks should show the project's interpreter as an option when you click the `kernel` icon or the small icon showing the current version of python (e.g., `Python 3.12.1`) and then click `Select Another Kernel`, and finally click `Python Environments...`.

## License

This repository is provided with an MIT license. See the `LICENSE` file.

## Contributing

Please email Mauro Sanchirico at ms3978@camden.rutgers.edu (academic) or sanchirico.mauro@gmail.com (personal) with questions, comments, bug reports, or suggestions for improvement.

