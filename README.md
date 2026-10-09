# HTTP Client

A minimal HTTP/1.0 client in C that fetches files from web servers over TCP.

## Overview
Built as part of Columbia University's Computer Systems course (COMS 3157). The client resolves a hostname via DNS, connects over TCP, sends an HTTP GET request, parses the response, and saves the file locally.

## Tech Stack
- **Language:** C
- **Protocols:** HTTP/1.0, TCP/IP, DNS
- **System Calls:** gethostbyname, socket, connect, send, recv

## Key Features
- **DNS resolution** via gethostbyname
- **HTTP GET request** construction with Host header
- **Response parsing:** status line check, header skipping, body extraction
- **Binary-safe** file download using fread/fwrite
- **Proper error handling** for connection failures, non-200 responses, and I/O errors

## Usage
