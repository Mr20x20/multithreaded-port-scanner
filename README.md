# Multithreaded TCP Port Scanner

A lightweight multithreaded TCP port scanner written in Python.

## Overview

This project scans a target host for open TCP ports within a specified range. The scanner uses Python threading and a task queue to improve scanning speed compared to a sequential implementation.

The project was built as a learning exercise to better understand:

* TCP communication
* Port scanning techniques
* Socket programming
* Multithreading in Python
* Network reconnaissance fundamentals

## Features

* TCP port scanning
* User-defined port range
* Multithreaded architecture
* Queue-based task distribution
* Execution time measurement
* Sorted output of discovered open ports

## Technologies Used

* Python 3
* socket
* threading
* queue

## Usage

Run the scanner with:

```bash
python port_scanner.py <IP_ADDRESS> <START_PORT> <END_PORT>
```

Example:

```bash
python port_scanner.py 192.168.1.1 1 1024
```

Example output:

```text
22/tcp OPEN
80/tcp OPEN
443/tcp OPEN

Found 3 open ports
Scan completed in 1.42 seconds
```

## Learning Objectives

The purpose of this project is educational. It was created to explore how TCP port scanning works at a low level and to gain practical experience with Python networking and concurrency.

## Future Improvements

* Service banner grabbing
* UDP scanning support
* Export results to file
* Custom thread count
* Host discovery module
* Service identification

## Disclaimer

This tool is intended for educational purposes and authorized security testing only. Do not scan systems without permission.
