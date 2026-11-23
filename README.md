# python-vpn

VPN research often requires a server implementation whose source you can inspect and modify. python-vpn is a VPN server implemented in pure Python, based on qwj/python-vpn.

**For research purposes only.** The available project information does not establish production readiness or security guarantees.

## Features

- Run a VPN server implemented in pure Python.
- Inspect and modify the Python implementation for VPN research.
- Reuse the code under the MIT license, subject to its copyright and license notice requirements.

## Installation

From a local checkout of python-vpn, create an isolated Python environment:

```sh
cd python-vpn
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
```

On Windows, activate the environment with `.venv\Scripts\activate` instead.

The supplied project information does not specify dependencies, a supported Python version, or a package installation method. Check the source tree for dependency declarations before installing additional packages.

## Usage

**The server entry point and command-line options have not been verified.** The following is a command template, not a confirmed invocation:

```sh
python path/to/vpn_server.py --help
```

Replace `path/to/vpn_server.py` with the actual server script. Use `--help` only if that entry point supports it. Confirm the required configuration and launch arguments in the source before starting the server in an isolated test environment.

The donor metadata lists IPsec, IKEv1, IKEv2, ESP, PSK, and WireGuard as topics. Those tags alone do not establish which protocols or configuration options this standalone project supports.

## License

MIT. python-vpn is based on [qwj/python-vpn](https://github.com/qwj/python-vpn), which is also MIT-licensed. Retain the upstream copyright notice and MIT permission notice in copies or substantial portions of the inherited code, and include them in this project's LICENSE file.

