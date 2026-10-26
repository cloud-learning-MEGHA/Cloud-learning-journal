# Networking Foundations — Revision

## 1. Private IP vs Public IP

- A private IP address identifies a device within its local network.
- A public IP address is used to communicate across the internet.
- Example of a private IP: `192.168.1.5`
- Example of a public IP: `203.0.113.10` (example address only).

## 2. DNS (Domain Name System)

- DNS helps find the IP address associated with a domain name.
- It allows us to use domain names instead of remembering IP addresses.
- When we open YouTube, DNS can help resolve its domain name to an IP address.

## 3. NAT (Network Address Translation)

- NAT translates IP addresses as traffic passes between networks.
- A home router commonly allows multiple devices to share one public IPv4 address using NAT.
- The router tracks translations so responses can reach the correct device.

## 4. What I Learned Today

When I open a website:
1. DNS helps resolve the website's domain name to an IP address.
2. My laptop uses its private IP on the local network.
3. The router uses NAT to send traffic towards the internet.
4. The router forwards the returning response to the correct device.


## DHCP (Dynamic Host Configuration Protocol)
- DHCP automatically provides network configuration to a device.
- It commonly provides an IP address, subnet mask, default gateway, and DNS server settings.
- It helps avoid IP address conflicts within its managed address pool.

## Default Gateway
- A default gateway helps a device communicate with destinations outside its local network.
- Devices on the same subnet can generally communicate directly without using the default gateway.
- On a phone hotspot, the phone's hotspot interface commonly acts as the laptop's default gateway.

## Phone Hotspot Data Flow

**When the phone uses Wi-Fi:**

Laptop → Phone → Wi-Fi Router → Internet → Server

**When the phone uses mobile data:**

Laptop → Phone → Mobile Network → Internet → Server

- The phone forwards the laptop's traffic through its available internet connection.
- NAT may translate the laptop's private IP traffic and track connections so responses can return to the correct device.
