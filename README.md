## Rethink DNS + Firewall + VPN for Android

The goal of this fork is to re-enable the option to use both Wireguard and SOCKS/HTTP Proxies, all other app functionality is identical to the current release.  This is a personal project but it's available for anyone else to use.  
Good for use cases like being able to run a VPN along side a Tailscale SOCKS proxy or connect something like orbot without giving up one or the other.

SOCKS/HTTP Proxies can be enabled to either be enabled for specific apps similarly to the settings for Orbot or can be globally enabled by not adding any apps.  If you choose to do a global enable you will need to put specific extension or IP to forward with an example being ts.net for tailscale traffic.

The current version is forked off the current latest rethink version.  It includes a preset for SOCKS and HTTP proxies to funnel tailscale, .onion, and .i2p traffic over them if they're enabled which can be modified to include more or less IPs and Domains to capture.  Anything not specified will be forwarded onto wireguard proxies if they're enabled.  

Thank you to the team developing RethinkDNS for all the hard work they've done on making something as useful as Rethink.
