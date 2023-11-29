# WebSocket Echo Test

## Overview

This repository contains a basic implementation of a WebSocket echo server and client. The server is written in Go, and the client uses JavaScript. This simple program allows you to send messages from the client to the server, and the server echoes the received messages back to the client.

## Table of Contents

- [Setup](#setup)
  - [Server-side (Go)](#server-side-go)
  - [Client-side (JavaScript)](#client-side-javascript)
- [Usage](#usage)
- [Notes](#notes)

## Setup

### Server-side (Go)

1. Make sure you have [Go](https://golang.org/) installed on your machine.

2. Clone the repository or download the `main.go` file.

3. Open a terminal and navigate to the directory containing `main.go`.

4. Run the following command to start the server:

   ```bash
   go run main.go
   ```
   This will start the server on localhost:1234.
### Client-side (JavaScript)

1. Open the `websocket.html` file in a web browser.
2. The web page contains a text input for entering messages and a "Send Message" button to send messages to the server.

## Usage

1. Open the client-side HTML file in a web browser.
2. Enter a message in the input field and click the "Send Message" button.
3. The message will be sent to the server, which will then echo it back to the client.
4. The echoed message will be displayed on the web page.

## Notes

- The server is implemented in Go and uses the `golang.org/x/net/websocket` package for WebSocket communication.
- The client-side uses JavaScript to create a WebSocket connection and send/receive messages.
- The server echoes the received messages back to the client.
- The server and client communicate over WebSocket protocol at ws://localhost:1234.
- The server-side Go code includes a simple goroutine (serveSide) to continuously read from the console and send messages to the connected WebSocket client. This is just for demonstration purposes and can be modified as needed.
