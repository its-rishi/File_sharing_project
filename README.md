# File Sharing Server

This project is a simple file-sharing server implemented in Python. It allows users to share the contents of their current directory over a local network using a built-in HTTP server. A QR code is generated to easily access the server from other devices on the same network.

## Features

- **Simple HTTP Server:** Shares the content of the current directory over HTTP.
- **QR Code Generation:** Generates a QR code that can be scanned to access the server.
- **Cross-Platform:** Works on Windows, macOS, and Linux.

## Prerequisites

- Python 3.x
- Required Python packages:
  - `pyqrcode`
  - `pypng` (for QR code generation)
  - `webbrowser` (to open the QR code image)

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/file-sharing-server.git
   cd file-sharing-server
   ```

2. **Install the required packages:**

   You can use `pip` to install the necessary packages:

   ```bash
   pip install pyqrcode pypng
   ```

## Usage

1. **Run the Server:**

   Navigate to the directory you want to share and run the script:

   ```bash
   python server.py
   ```

   The server will start and display your PC name, IP address, and the directory being shared.

2. **Access the Server:**

   - A QR code will be generated and saved as `myqr.png` in the current directory. Open this image, and scan the QR code with your mobile device to access the shared content.

   - Alternatively, enter the displayed IP address and port (e.g., `http://192.168.1.100:8080`) into a web browser on any device connected to the same network.

3. **Stopping the Server:**

   To stop the server, simply close the terminal or interrupt the process (Ctrl+C).

## Security Notice

This project is intended for use on local networks only. It does not include security features such as authentication or encryption. Be cautious when sharing sensitive data.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The project utilizes the `pyqrcode` library for QR code generation.
- It uses Python's built-in `http.server` module for serving files.

## Contributing

Feel free to open issues or submit pull requests if you have suggestions or improvements.
