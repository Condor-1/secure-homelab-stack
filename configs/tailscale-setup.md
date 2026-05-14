# Tailscale Setup

## Purpose

Tailscale is used to securely access the homelab environment remotely without exposing ports directly to the public internet

One of the main goals during setup was to make remote administration simple while still keeping the overall environment secure

---

## Configuration

The setup process included:-
- Installing Tailscale on Ubuntu Server
- Connecting devices to the private mesh network
- Enabling secure remote SSH access
- Testing remote connectivity between devices
- Configuring the server as an exit node during testing

Some additional troubleshooting was required during the initial setup phase to properly verify routing behavior and connectivity between devices

---

## Access Control

After the basic setup was working, additional time was spent configuring access permissions properly inside the Tailscale dashboard

Administrative access is restricted to trusted accounts only

Devices connected for testing purposes are limited to using network services without access to:-
- Server administration
- Remote management
- Security dashboards
- Configuration settings

This separation helped reduce unnecessary administrative exposure and made the environment safer to test with additional devices

---

## SSH Improvements

To make remote administration easier, SSH key-based authentication was configured for the main management system

This included:-
- Generating public/private SSH key pairs
- Adding trusted device authentication
- Reducing repeated password usage during administration

This significantly improved both convenience and security while managing the server remotely

---

## Benefits

Using Tailscale provided several advantages during the project:-
- Secure encrypted communication
- Simplified remote access
- Safer alternative to direct port forwarding
- Easier remote management from multiple devices

---

## Notes

Authentication details, network identifiers, and sensitive configuration information have been removed from public documentation
