# Networking Commands

1. **`ping google.com`** – Checks connectivity to a remote server.
2. **`ifconfig`** – Displays network interfaces (deprecated, use `ip`).
3. **`ip a`** – Shows IP addresses of network interfaces.
4. **`netstat -tulnp`** – Displays open network connections.
5. **`curl https://example.com`** – Fetches a webpage's content.
6. **`wget https://example.com/file.zip`** – Downloads a file from the internet.


### Network Monitoring
- `ifconfig` – Show network interfaces (deprecated, use `ip a`)
- `ip a` – Show network interface details
- `netstat -tulnp` – Show active connections and listening ports
- `ss -tulnp` – Alternative to `netstat` for socket statistics
- `ping hostname` – Test network connectivity
- `traceroute hostname` – Show network path to a host
- `nslookup domain` – Get DNS resolution details

## Network Monitoring
### Checking Network Interfaces
```bash
ip a  # Show IP addresses and interfaces
```
### Viewing Open Ports and Connections
```bash
netstat -tulnp  # Show listening ports
ss -tulnp  # Alternative to netstat
```
### Testing Connectivity
```bash
ping google.com  # Test internet connection
traceroute google.com  # Trace the path to Google
```
### Checking DNS Resolution
```bash
nslookup example.com
```
