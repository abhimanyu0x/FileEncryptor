# File Encryptor & Decryptor

This project is a C++ implementation of a file encryption and decryption tool. It allows users to encrypt or decrypt files in a specified directory.

## Project Overview

The File Encryptor & Decryptor is designed to process multiple files in a given directory, either encrypting or decrypting them based on user input. The project utilizes modern C++ features and follows a modular architecture for efficient file processing.

### Key Components

1. **IO**: Handles file input/output operations.
2. **ProcessManagement**: Manages the queuing and execution of encryption/decryption tasks.
3. **Task**: Represents an individual encryption or decryption task for a file.

## How It Works

1. The user provides a directory path and specifies the action (encrypt or decrypt).
2. The program recursively iterates through the directory, creating a task for each file.
3. Tasks are submitted to a queue managed by the ProcessManagement component.
4. Child processes are spawned to perform the actual encryption or decryption operations.
5. The ProcessManagement component handles task execution and inter-process communication.

## Features

- Recursive directory traversal
- Multi-process execution for improved performance
- Support for both encryption and decryption operations
- Error handling for filesystem operations

## Usage

Compile the project and run the executable. When prompted:

1. Enter the directory path containing the files you want to process.
2. Specify the action: "encrypt" or "decrypt".

The program will then process all files in the given directory and its subdirectories.

## Dependencies

- C++17 or later (for std::filesystem support)
- Standard C++ libraries

## Future Improvements

- Add support for custom encryption algorithms
- Implement progress reporting
- Add command-line argument parsing for non-interactive use

## Contributing

Contributions to improve the project are welcome. Please feel free to submit issues or pull requests.
