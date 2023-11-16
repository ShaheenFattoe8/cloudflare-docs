---
_build:
  publishResources: false
  render: never
  list: never
---

* Load Balancing [session affinity](/load-balancing/understand-basics/session-affinity/), [failover across pools](/load-balancing/understand-basics/adaptive-routing/#failover-across-pools), and [custom rules](/load-balancing/additional-options/load-balancing-rules/) are not supported by Spectrum.

* UDP health checks are only available with public monitoring. TCP can be used with both public and private monitoring.