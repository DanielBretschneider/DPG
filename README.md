# DPG – Daniel's Password Generator

A lightweight, secure and easy-to-use command-line password generator written in Go.

## Overview

**DPG (Daniel's Password Generator)** is a small command-line utility designed to generate secure random passwords directly from your terminal.

The goal is to create a simple, flexible and reliable tool that can be executed from anywhere in the Linux system without having to navigate to the project directory.

Users will be able to customize password length, character sets and the number of passwords generated through command-line arguments.

## Features

Planned features:

- Generate cryptographically secure random passwords.
- Customize password length.
- Include or exclude uppercase letters.
- Include or exclude lowercase letters.
- Include or exclude numbers.
- Include or exclude special characters.
- Exclude specific characters.
- Generate multiple passwords in a single execution.
- Execute globally from any terminal location.

## Usage

### Basic password generation

Generate a password using the default configuration:

```bash
dpg
```

### Customize password length

```bash
dpg --length 32
```

### Include special characters

```bash
dpg --length 24 --symbols
```

### Generate multiple passwords

```bash
dpg --count 5
```

### Exclude specific characters

```bash
dpg --exclude "0OIl"
```

## Command-line options

| Option | Description | Default |
|---|---|---|
| `-l`, `--length` | Password length | 16 |
| `-u`, `--uppercase` | Include uppercase letters (A-Z) | Enabled |
| `-L`, `--lowercase` | Include lowercase letters (a-z) | Enabled |
| `-n`, `--numbers` | Include numbers (0-9) | Enabled |
| `-s`, `--symbols` | Include special characters | Disabled |
| `-e`, `--exclude` | Characters to exclude | None |
| `-c`, `--count` | Number of passwords to generate | 1 |
| `-h`, `--help
