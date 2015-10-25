Message Persistence
===================

- **4.0.1** ![](/badge/rec.png) A client should provide the ability to save its
  message history, and provide a persistent view of that history across client
  restarts.

- **4.0.2** ![](/badge/rec.png) Message persistence should be disabled by
  default.
  - Clients may provide users with a setting to enable message persistence by
    default.
  - If stored message logs are not encrypted, clients must make the user aware
    of this fact if they enable message persistence.

- **4.0.3** ![](/badge/req.png) If message persistence is enabled by default,
  all message logs stored on the device must be encrypted using the cryptography
  functions provided by the Tox API, or a comparably reputable, free and open
  source cryptography library.
