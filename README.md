# LTSA — Labelled Transition System Analyser

A verification tool for concurrent systems, with a working Message Sequence Chart (MSC) plugin.

## Table of Contents
- [LTSA — Labelled Transition System Analyser](#ltsa--labelled-transition-system-analyser)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Plugins](#plugins)
  - [Installation](#installation)
    - [Windows](#windows)
    - [Linux (Ubuntu)](#linux-ubuntu)
    - [Troubleshooting (Linux)](#troubleshooting-linux)
    - [Java Requirement](#java-requirement)
  - [Manual](#manual)

## Overview

LTSA (Labelled Transition System Analyser) is a verification tool for concurrent systems. It automatically checks whether the specification of a concurrent system satisfies its required behavioral properties, and supports specification animation for interactive exploration of how a system behaves.

The Message Sequence Chart (MSC) plugin extends LTSA with the ability to graphically edit sets of scenarios and construct message sequence charts, offering a visual way to explain models. As part of an iterative design process, LTSA can also help surface implied behavior within a system.

This repository contains an extended version of LTSA with a working MSC plugin.

> **Note:** The [official LTSA release](https://www.doc.ic.ac.uk/ltsa) was last updated in June 2006, and its additional plug-ins are no longer functional.

## Plugins

LTSA includes the following plugins. See the [official documentation](https://www.doc.ic.ac.uk/ltsa) for full details on each.

- **MSC** — Message Sequence Chart editor, described in the [Overview](#overview) above
- **Scenebeans**
- **Web**

## Installation

### Windows
1. Download the Windows release as a ZIP file.
2. Unzip the archive and run `run.cmd`.
3. LTSA will start automatically.

### Linux (Ubuntu)
1. Download the Linux (Ubuntu) release as a ZIP file.
2. Unzip the archive.
3. Open a terminal in the extracted folder and run:

   ```bash
   find . \( -type d -exec chmod 755 {} \; -o -type f -exec chmod 644 {} \; \) && chmod +x run.sh install.sh uninstall.sh jre/bin/java
   ```

   ```bash
   sudo ./install.sh
   ```

4. Start LTSA by running:

   ```bash
   ./run.sh
   ```

   Alternatively, right-click `run.sh` and select **Run as a Program**.

### Troubleshooting (Linux)
If you run into issues launching LTSA:
1. Update your system:

   ```bash
   sudo apt update && sudo apt upgrade
   ```

2. Reboot your device.
3. Uninstall LTSA:

   ```bash
   sudo ./uninstall.sh
   ```

4. Repeat the [Linux installation](#linux-ubuntu) steps above.

### Java Requirement
If you're still having trouble running the tool, make sure Java is installed. You can download it from the [official Java website](https://www.java.com/download/ie_manual.jsp).

## Manual

To access the built-in manual:
1. Start LTSA.
2. Open the **Help** menu in the toolbar.
3. Select **Manual**.
