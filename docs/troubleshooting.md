# Troubleshooting Notes

## Initial Tailscale Exit Node Setup

Setting up the Tailscale exit node took more trial and error than expected. Getting remote traffic to properly route through the homelab environment required multiple rounds of testing and reconnecting devices

### Challenges:-
- Route configuration inconsistencies
- Connectivity verification between devices
- Devices not always following expected routing behavior

### Resolution:-
- Rechecked Tailscale route settings multiple times
- Re-authenticated connected devices
- Tested traffic flow between systems until routing worked consistently

---

## IP Address Mismatches

During setup, some services occasionally showed inconsistent local IP behavior, which caused confusion while troubleshooting connectivity issues

### Resolution:-
- Verified static local addressing
- Double-checked DNS configuration
- Restarted affected services and devices
- Re-tested connectivity after changes

---

## SSH Authentication Improvements

Typing passwords repeatedly during remote administration quickly became frustrating while working on the server regularly

### Resolution:-
- Configured SSH key-based authentication
- Generated public/private SSH key pairs
- Added trusted device configuration for the main administration PC

This made remote administration much smoother while also improving security

---

## Pi-hole DNS Filtering Issues

One of the biggest headaches during setup was getting devices to consistently route DNS traffic through Pi-hole. Some devices continued using external DNS services, which meant ads and trackers were still getting through

### Resolution:-
- Renewed DNS leases on devices
- Reconfigured DNS settings manually where required
- Verified DNS requests through the Pi-hole dashboard
- Tested filtering functionality repeatedly after configuration changes

---

## CrowdSec Whitelisting Adjustments

After enabling CrowdSec monitoring, some trusted local services and devices started generating unnecessary alerts during testing

### Resolution:-
- Added basic whitelist rules for Pi-hole and Tailscale-related activity
- Reduced false positives from trusted systems
- Improved monitoring stability without interfering with normal usage

---

## Tailscale Access Control Configuration

The Tailscale access control setup was initially confusing because of the UI and permission structure. Extra testing was needed to properly separate normal users from administrative access

### Resolution:-
- Restricted administrative access to trusted accounts only
- Limited connected test devices to service usage without management permissions
- Verified separation between client access and server administration
