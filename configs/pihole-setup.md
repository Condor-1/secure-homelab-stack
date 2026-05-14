# Pi-hole Setup

## Purpose

Pi-hole is used for network-wide DNS filtering and advertisement blocking across connected devices inside the homelab environment

One of the main goals of this setup was to reduce advertisements, trackers, and unnecessary DNS traffic while also learning more about how DNS routing works in a real-world environment

---

## Installation

Pi-hole was installed on Ubuntu Server using the official installation method

The service was deployed on the headless server environment and configured to run continuously as part of the 24/7 homelab setup

---

## Configuration

The initial configuration process included:-
- Setting a static local IP address
- Configuring upstream DNS providers
- Enabling dashboard access
- Connecting client devices to use Pi-hole for DNS resolution

Additional testing and troubleshooting were required during setup because some devices initially continued bypassing Pi-hole and using external DNS services

---

## DNS Troubleshooting

One of the more time-consuming parts of the setup was ensuring DNS requests consistently passed through Pi-hole correctly

Some devices initially:-
- Ignored configured DNS settings
- Continued using cached DNS information
- Bypassed filtering functionality entirely

### Resolution

To resolve these issues:-
- DNS leases were renewed
- Device DNS settings were reconfigured
- Filtering activity was verified through the Pi-hole dashboard
- Multiple rounds of testing were performed after configuration changes

---

## Features Used

Current Pi-hole functionality includes:-
- DNS filtering
- Advertisement and tracker blocking
- Query logging
- Dashboard monitoring
- Basic whitelist management for trusted services

---

## Benefits

Using Pi-hole helped improve:-
- Network-wide advertisement blocking
- Visibility into DNS activity
- Control over DNS filtering behavior
- Understanding of DNS request routing and management

---

## Notes

Sensitive configuration details, DNS records, and IP addresses have been removed from public documentation
