# Rusty-Journal

## Index
- [Rusty-Journal](#rusty-journal)
  - [Index](#index)
  - [Introduction](#introduction)
  - [Requirements](#requirements)
  - [Features](#features)
  - [Technologies](#technologies)
  - [Build instructions](#build-instructions)
  - [Further information](#further-information)

## Introduction
**Rusty-Journal** is a CLI tool created for task handling. The main goal behind this project is to learn Rust and get familiarized with Cargo and the Crates system. 


## Requirements
You just need to have installed Cargo and Rust. You can do this with the following [tutorial](https://www.rust-lang.org/tools/install), using rustup.

## Features
- Show help
    ```bash
    cargo run --
    ```

- List all tasks stored in a journal
    ```bash
    cargo run -- -j .journal.json list
    ```

- Create a new task in the desired journal
    ```bash
    cargo run -- -j .journal.json add 'take a walk'
    ```

- Remove a task from the journal specifying its position
    ```bash
    cargo run -- -j .journal.json complete 1
    ```

**Note:** If the journal file is omitted it takes `.journal.json` by default, which should be present at the user's home directory.

## Technologies

-   [Rust](https://www.rust-lang.org/)
-   [StructOpt](https://github.com/TeXitoi/structopt)
-   [Chrono](https://github.com/chronotope/chrono)
-   [Serde_Json](https://docs.rs/serde_json/latest/serde_json/)
-   [Home](https://docs.rs/home/latest/home/)
-   [AnyHow](https://github.com/dtolnay/anyhow)

## Build instructions
To compile the program, go to the terminal and run the command `cargo run --release`.

The compiled binary (the executable file) will be in the `target/release/` directory and will be named after the project name. If you're using macOS or Linux, it will be called rusty-journal. If you're using Windows, it will be called rusty-journal.exe.

You can call it from your command-line directly now. No need for Cargo anymore! Just make sure its directory is listed in your `PATH` environment variable.

## Further information
-   [Full Course](https://learn.microsoft.com/en-us/training/paths/rust-first-steps/)
-   [Tutorial](https://learn.microsoft.com/en-us/training/modules/rust-create-command-line-program/)