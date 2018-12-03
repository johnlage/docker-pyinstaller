# PyInstaller Docker Images

**johnlage/pyinstaller-linux** and **johnlage/pyinstaller-windows** are a pair of Docker containers to ease compiling Python applications to binaries / exe files.
(Based on/Forked from cdrx/pyinstaller-linux and cdrx/pyinstaller-windows, but up to date with both Python 3.7 for py3 and PyInstaller 3.4, as well as repurposed for CI use.)

Current PyInstaller version used: 3.4.

## Tags

`johnlage/pyinstaller-linux` and `johnlage/pyinstaller-windows` both have two tags, `:python2` and `:python3` which you can use depending on the requirements of your project. `:latest` points to `:python3`

The `:python2` tags run Python 2.7.

The `:python3` tag runs Python 3.6 on Linux and Python 3.6 on Windows.

## Usage

There are two containers, one for Linux and one for Windows builds. The Windows builder runs Wine inside Ubuntu to emulate Windows in Docker.

These are currently meant to be used for CI builds (for example through GitLab CI)

## History

See the Commit History and the old version [here](https://github.com/cdrx/docker-pyinstaller).

## License

MIT
