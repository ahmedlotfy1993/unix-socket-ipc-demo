# unix-socket-ipc-demo
This project demonstrates **Inter-Process Communication (IPC)** on a Linux system using **AF_UNIX (Unix Domain Sockets)**.  
It consists of a simple **server** and **client** program:

- The **client** sends integers to the server.  
- When the client enters `0`, it stops sending numbers and requests the result.  
- The **server** receives the integers, calculates their sum, and sends the final result back to the client.  

This example is useful for learning about:
- Local IPC using Unix domain sockets.
- Basic socket programming (`socket`, `bind`, `listen`, `accept`, `connect`, `read`, `write`).
- Building and running C projects with **CMake**.

---

## 📂 Project Structure
- CMakeLists.txt # CMake build configuration
#  📂 AF_UNIX
- client.c # Client application
- server.c # Server application
---

## ⚙️ Requirements

- Linux system with support for Unix Domain Sockets (all modern distros).
- A C compiler (`gcc` or `clang`).
- CMake version **3.10+**.
- Basic development tools:
  ```bash
  sudo apt update
  sudo apt install build-essential cmake -y   # Ubuntu/Debian
  git clone https://github.com/your-username/unix-socket-ipc-demo.git
  cd unix-socket-ipc-demo
  mkdir build && cd build
  cmake ..
  ./build/server
  ./build/client
  ```
