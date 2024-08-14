# MongoDB ObjectId Tools

Welcome to the MongoDB ObjectId Tools! This project provides two simple yet 
powerful tools for working with MongoDB ObjectIds:

- **ObjectId Decoder:** Decode a MongoDB ObjectId to reveal its underlying 
  components.
- **ObjectId Encoder:** Generate a valid MongoDB ObjectId by specifying its 
  components.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
  - [ObjectId Decoder](#objectid-decoder)
  - [ObjectId Encoder](#objectid-encoder)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Introduction

MongoDB uses ObjectIds as unique identifiers for documents within collections. 
These 12-byte values are typically composed of:

- A 4-byte timestamp (in seconds since the Unix epoch)
- A 3-byte machine identifier
- A 2-byte process identifier
- A 3-byte counter

This project provides an interactive way to both decode and encode MongoDB 
ObjectIds, making it easier to understand and manipulate these identifiers.

## Features

- **ObjectId Decoder:** Input a MongoDB ObjectId and decode it to extract the 
  timestamp, machine identifier, process identifier, and counter.
- **ObjectId Encoder:** Generate a MongoDB ObjectId by specifying the timestamp, 
  machine identifier, process identifier, and counter.

## Installation

To use this project, simply clone the repository and open the `index.html` file 
in your browser. No additional setup or dependencies are required.

```bash
git clone https://github.com/ExZyle/mongo-objectid-tools.git
cd mongo-objectid-tools
```

# Usage

## ObjectId Decoder

1. Navigate to the decoder.html page.
2. Enter a valid MongoDB ObjectId in the input field.
2. Click "Decode" to reveal the decoded components, including the timestamp 
   (in both UTC and local time), machine identifier, process identifier, 
   and counter.

## ObjectId Encoder

1. Navigate to the encoder.html page.
2. Provide the following details:
3. Timestamp: Select the date and time (local time zone).
4. Machine Identifier: Enter a 6-character hexadecimal string.
5. Process Identifier: Enter a number between 0 and 65535.
6. Counter: Enter a number between 0 and 16777215.
7. Click "Generate ObjectId" to create and display the ObjectId based on the 
   provided inputs.

# Project Structure

The project consists of three main HTML files:

* `index.html`: The landing page with instructions and links to the tools.
* `decoder.html`: The page for decoding MongoDB ObjectIds.
* `encoder.html`: The page for encoding MongoDB ObjectIds.

```
mongo-objectid-tools/
│
├── index.html
├── encoder.html
├── decoder.html
└── README.md
```

# Contributing

Contributions are welcome! If you'd like to improve this project, please fork 
the repository and create a pull request. For major changes, please open an 
issue first to discuss what you'd like to change.

1. Fork the project
2. Create your feature branch (git checkout -b feature/AmazingFeature)
3. Commit your changes (git commit -m 'Add some AmazingFeature')
4. Push to the branch (git push origin feature/AmazingFeature)
5. Open a pull request

# License

This project is licensed under the MIT License. See the [LICENSE](LICENCE.md) 
file for details.
