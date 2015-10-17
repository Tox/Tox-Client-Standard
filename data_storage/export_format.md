Export Format
-------------

- **5.1.1** ![](/badge/req.png) A Toxcore data file saved in the root of the client's
  working directory, with the file name `<profile_name>.tox`

- **5.1.2** ![](/badge/req.png) If the client supports user avatars, they will be stored
  under the `avatars/` directory in the root of the client's working directory.

- **5.1.3** ![](/badge/req.png) Avatars are named according to the following format:
  `PK.png`, where PK is the 64-character hexadecimal public key of its owner.

- An example file heirarchy:

  ```
  +-----------------------------------------------------------------------------------+
  |   / (client working dir)                                                          |
  |    |                                                                              |
  |    +-- tox_save.tox                                                               |
  |    +-- avatars/                                                                   |
  |         |                                                                         |
  |         +-- E62DACF4C0DD23156F745874CBDBCD3D3E356F51C67921F7D91A7938CEB87933.png  |
  |         +-- DD2A1340FECE441206B5F3D202E6146E76617270214499B72C5511FCE839F85B.png  |
  +-----------------------------------------------------------------------------------+
  ```
