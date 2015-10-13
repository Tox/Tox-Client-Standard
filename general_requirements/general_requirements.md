General Requirements
====================

- ![](badge/req.png) Clients must not use any form of unencrypted
  communication.

- ![](badge/req.png) If a client is configured to use a proxy, but is not also
  configured to use a forced TCP connection, it must warn the user that their
  IP address may not be hidden.

- ![](badge/req.png) When a client is configured to use a proxy, and is also
  configured to force a TCP connection, all traffic that does not use the proxy
  must be blocked, including (but not limited to) DNS and HTTPS-based username
  lookups.

- ![](badge/req.png) All features supported by the tox.h and toxav.h APIs that
  are used by the client must be fully functional without the usage of
  third-party services.
