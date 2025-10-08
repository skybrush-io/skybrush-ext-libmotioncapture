libmotioncapture extension for Skybrush Server
==============================================

This repository contains an experimental extension module to Skybrush Server
that adds support for multiple mocap systems via an abstraction layer offered
by `libmotioncapture` for indoor drone tracking.

Installation
------------

1. Check out this repository using git.

2. Install [`uv`](https://astral.sh/uv) if you haven't done so yet;
   `uv` is a tool that allows you to install Skybrush Server and the
   extension you are working on in a completely isolated virtual environment.

3. Run `uv sync`; this will create a virtual environment and install
   Skybrush Server with all required dependencies in it, as well as the code
   of the extension.

4. Modify `skybrushd.jsonc` to point to the host where the Qualisys Track
   Manager app is running.

5. In the shell prompt, type `uv run skybrushd -c skybrushd.jsonc` to start
   the server with a configuration file that loads the extension.
