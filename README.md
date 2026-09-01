# IvyWire
It is a framework for RaspberryPi's and other SBCs to communicate with each other to send data or to cluster together

**Status:** 🚧 Proof of Concept

---

## Overview

IvyWire is a framework designed to allow multiple single-board computers (SBCs) to communicate with one another and work together in a cluster or to simply transfer data between two or more SBC's.

The goal is to make it possible to connect devices such as Raspberry Pis and other SBCs into a cluster that can:

* Communicate between nodes
* Share data
* Discover other nodes
* Distribute tasks
* Work together as a single system

This project is currently a **proof of concept** and is under active development.

---

## How It Works

A cluster consists of multiple independent nodes connected over a network.

```text
                 ┌──────────────┐
                 │    Node 1    │
                 │ Raspberry Pi │
                 └───────┬──────┘
                         │
              ┌──────────┼──────────┐
              │          │          │
        ┌─────▼─────┐ ┌──▼───────┐ ┌▼──────────┐
        │   Node 2  │ │  Node 3  │ │   Node 4  │
        │ Raspberry │ │   SBC    │ │ Raspberry │
        │     Pi    │ │          │ │    Pi     │
        └───────────┘ └──────────┘ └───────────┘
```

Each node runs the framework and communicates with other nodes using [communication method/protocol].


## Supported Hardware

All Raspberry Pi's that support python 3.9+

### Tested

* Raspberry Pi 4b 

### Planned / Untested

* all full fledge Raspberry Pi's and compute modules (not pico or zero models)

Hardware listed as untested may work, but has not been verified.

---

## Requirements

* Python 3.9+
* Network connection
* 5MB of storage

---

**Node**
: An individual SBC running the framework.

**Cluster**
: A collection of connected nodes.

---

## Contributing

This project is currently a proof of concept, but ideas, bug reports, testing, and contributions are welcome.

If you find a bug or have an idea for a feature, please open an issue.

---

## License

This project is licensed under the **MIT License**.

See the LICENSE file for the full license text.

---

## Disclaimer

This project is experimental software.

It is currently a proof of concept and may contain bugs, incomplete features, breaking changes, or other issues. Do not rely on it for critical systems.

---

## Author

Created by **SudoCherry]**.

First Contribution: 1/9/2026
