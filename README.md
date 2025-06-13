<h1 align="center">
  <br>
  <a href="https://jonasheinle.de"><img src="images/logo.png" alt="logo" width="200"></a>
  <br>
  RaspberryPiBrowserLivestream
  <br>
</h1>

<h4 align="center">This repo achieves a livestream from a raspberry pi to a browser.<a href="https://jonasheinle.de" target="_blank"></a>.</h4>

[![Ubuntu 24.04 Workflow](https://github.com/Kataglyphis/RaspberryPiBrowserLivestream/actions/workflows/ubuntu-24.04.yml/badge.svg)](https://github.com/Kataglyphis/RaspberryPiBrowserLivestream/actions/workflows/ubuntu-24.04.yml)
[![Windows 2025 Workflow](https://github.com/Kataglyphis/RaspberryPiBrowserLivestream/actions/workflows/windows-2025.yml/badge.svg)](https://github.com/Kataglyphis/RaspberryPiBrowserLivestream/actions/workflows/windows-2025.yml)
[![Ubuntu 24.04 ARM Workflow](https://github.com/Kataglyphis/RaspberryPiBrowserLivestream/actions/workflows/ubuntu-24.04-arm.yml/badge.svg)](https://github.com/Kataglyphis/RaspberryPiBrowserLivestream/actions/workflows/ubuntu-24.04-arm.yml)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/paypalme/JonasHeinle)
[![Twitter](https://img.shields.io/twitter/follow/Cataglyphis_?style=social)](https://twitter.com/Cataglyphis_)

<p align="center">
  <a href="#about-the-project">About The Project</a> •
  <a href="#overview">Overview</a> •
  <a href="#getting-started">Getting Started</a> •
  <a href="#tests">Tests</a> •
  <a href="#roadmap">Roadmap</a> •
  <a href="#contributing">Contributing</a> •
  <a href="#license">License</a> •
  <a href="#acknowledgements">Acknowledgements</a> •
  <a href="#literature">Literature</a>
</p>

<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#key-features">Key Features</a></li>
        <li><a href="#dependencies">Dependencies</a></li>
        <li><a href="#useful-tools">Useful Tools</a></li>
      </ul>
    </li>
    <li><a href="#overview">Overview</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#setup">Setup</a></li>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#deployment-recommendations-hardwaresoftware">Deployment Recommendations</a></li>
      </ul>
    </li>
    <li><a href="#tests">Tests</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact-and-maintainers">Contact and Maintainers</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
    <li><a href="#literature">Literature</a></li>
    <li><a href="#demo">Demo</a></li>
    <li><a href="#references">References</a></li>
    <li><a href="#known-issues">Known Issues</a></li>
  </ol>
</details>

---

## About The Project

This project provides a Python package named **RaspberryPiBrowserLivestream**.  
Use it to livestream your raspberry pi to a browser.

### Key Features

- Features are to be adjusted to your own project needs.


<div align="center">


|            Category           |           Feature                             |  Implement Status  |
|-------------------------------|-----------------------------------------------|:------------------:|
|  **Packaging agnostic**       | Binary only deployment                        |         ✔️         |
|                               | Lore ipsum                                    |         ✔️         |
|  **Streaming**                |                                               |                    |
|                               | flask support                                 |         ✔️         |
|  **Testing**                  |                                               |                     |
|                               | Advanced unit testing                         |         🔶         |
|                               | Advanced performance testing                  |         🔶         |
|                               | Advanced fuzz testing                         |         🔶         |

</div>

**Legend:**
- ✔️ - completed  
- 🔶 - in progress  
- ❌ - not started


### Dependencies

- Adjust according to your project’s actual Python and library dependencies.

### Useful Tools

| Tool                                               | Description             |
| -------------------------------------------------- | ----------------------- |
| [ty](https://github.com/astral-sh/ty)              | ty                      |
| [ruff](https://github.com/astral-sh/ruff)          | Linter                  |
| [uv](https://github.com/astral-sh/uv)              | Command-line utility    |
| [kedro](https://kedro.org/)                        | Infrastructure          |
| [Scalene](https://github.com/plasma-umass/scalene) | Benchmarking            |
| [py-spy](https://github.com/benfred/py-spy)        | Benchmarking            |

---

## Overview

The versioning of the package can be viewed in [CHANGELOG.md](CHANGELOG.md).

---

## Getting Started

### Setup

Feel free to adjust for your own environment.

#### Picamera web browser live stream

You need to shared system packages for the 
`picamera2` should be installed via `apt`
([source](https://github.com/raspberrypi/picamera2))

```bash
sudo apt install python3-picamera2
uv venv --system-site-packages
```

### Installation

There are three major ways to install this package in your environment:

1. **Install directly via pip:**
   ```bash
   pip install KataglyphisPythonPackage@git+https://github.com/Kataglyphis/RaspberryPiBrowserLivestream
   ```
   or install a specific tagged version:
   ```bash
   pip install KataglyphisPythonPackage@git+https://github.com/Kataglyphis/RaspberryPiBrowserLivestream@v0.0.1
   ```

2. **Install after cloning the repo:**
   ```bash
   git clone https://github.com/Kataglyphis/RaspberryPiBrowserLivestream
   pip install .
   ```

   or

   ```bash
   pip install -e .
   ```

   (an editable install: changes in the repo will be reflected in your environment)

3. **Add as a submodule to your repository:**
   ```bash
   git submodule add https://github.com/Kataglyphis/RaspberryPiBrowserLivestream
   ```
   Make sure that all dependencies are installed during your repo’s installation.  
   (Not generally recommended, as it can be more complicated.)

### Deployment Recommendations (Hardware/Software)

For insights into deploying Python packages into production as “binary only” wheels
have a look into the corresponding workflows.

---

## Tests

For development, you can install comprehensive dependencies with:
```bash
pip install -v -e .[docs,test,fuzzytest]
```
Then run your testing framework (e.g., `pytest`).

---

## Roadmap

Specify planned features or improvements here.

---

## Contributing

Contributions make open source software better! To contribute:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## License

Use or adapt your license here.

---

## Contact and Maintainers

- Primary contact: [@Cataglyphis_](https://twitter.com/Cataglyphis_)
- Project example link: [GitHub](https://github.com/Kataglyphis/...)

**Maintainers:**  
Replace this text with the list of maintainers who can be asked and assigned to review or merge requests.

---

## Acknowledgements

Mention credits for any third-party resources.

---

## Literature

List helpful literature, tutorials, or references that have guided this project.

---

## Demo

If you have examples or demonstrations, add them here.

---

## References

KataglyphisPythonPackage is used in the following repos/packages:
- Adapt this list to reference actual uses.

---

## Known Issues

List any known issues here. 
