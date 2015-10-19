General Requirements
====================

- **1.0.1** ![](/badge/req.png) Clients must not use any form of unencrypted
  communication.

- **1.0.2** ![](/badge/req.png) If a client is configured to use a proxy, but is not also
  configured to use a forced TCP connection, it must warn the user that their
  IP address may not be hidden.

- **1.0.3** ![](/badge/req.png) When a client is configured to use a proxy, and is also
  configured to force a TCP connection, all traffic that does not use the proxy
  must be blocked, including (but not limited to) DNS and HTTPS-based username
  lookups.

- **1.0.4** ![](/badge/req.png) All features supported by the tox.h, toxav.h and
  toxencryptsave.h APIs that are used by the client must be fully functional without
  the usage of third-party services.
