---
_build:
  publishResources: false
  render: never
  list: never
---

As a best practice, we also recommend that you explicitly block all traffic that does not come from Cloudflare IP addresses or the IP addresses of your trusted partners, vendors, or applications.

For example, you might [update your iptables](https://www.linode.com/docs/guides/control-network-traffic-with-iptables/#block-or-allow-traffic-by-port-number-to-create-an-iptables-firewall) with the following commands:

```sh
# For IPv4 addresses
$ iptables -A INPUT -p tcp -m multiport --dports http,https -j DROP
# For IPv6 addresses
$ ip6tables -A INPUT -p tcp -m multiport --dports http,https -j DROP
```

For more specific guidance, contact your hosting provider or website administrator.
