# Go Calculator Application

A simple command-line calculator application written in Go that performs basic arithmetic operations.

## Features

- Performs addition, subtraction, multiplication, and division
- Interactive command-line interface
- Type 'exit' to quit the application

## How It Works

The application prompts the user to enter a calculation in the format:
```
number operator number
```

For example:
```
1 + 2
5 - 3
4 * 6
8 / 2
```

Make sure to include spaces between the numbers and the operator as shown in the examples.

## Docker Setup

This application is containerized using Docker with a multi-stage build process to create a minimal image.

### Building the Docker Image

To build the Docker image, run the following command from the project directory:

```bash
docker build -t golang-calculator .
```



### Running the Docker Container

To run the application in a Docker container:

```bash
docker run -it golang-calculator
```

The `-it` flags are necessary to provide an interactive terminal for the calculator application.


## Development

The application is built using Go and consists of a simple main.go file that handles user input and performs calculations.

To run the application locally without Docker (requires Go installed):

```bash
go run main.go
```