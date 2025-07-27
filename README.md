# Ping-Optimizer-Morocco



## About This Project

**Ping-Optimizer-Morocco** is a Windows desktop application designed to optimize and manage your Cloudflare WARP VPN connection. It automatically selects the best network endpoint based on latency and packet loss, and connects you to your preferred Cloudflare data centers (colo) — specifically targeting **LIS** (Lisbon) or **MAD** (Madrid) locations.

The application features a modern and easy-to-use graphical interface built with Python and Tkinter, offering real-time logs, current colo status, and flexible configuration of target colos.

---

## Features

- Automatically disconnects any existing WARP session before optimization.
- Uses `warp.exe` in MASQUE mode to test multiple endpoints and selects the best one based on network latency and packet loss.
- Continuously retries connection until the current colo matches your preferred locations (`LIS` or `MAD` by default).
- Displays real-time logs and current colo status in a clean GUI.
- Allows users to customize target colo locations dynamically.
- Supports dark and light themes for comfortable use.
- Optional system tray integration (requires additional dependencies).
- Cross-platform compatible Python code (though optimized for Windows).

---

## Requirements

- Windows OS
- Python 3.7+
- `warp.exe` accessible in the same folder or system PATH
- Python packages:
  - `requests`
  - `pystray` (optional, for system tray)
  - `Pillow` (optional, dependency for pystray)

Install dependencies with:

```bash
pip install requests pystray pillow
