Export Format
-------------

- ![](/badge/req.png) A Toxcore data file saved in the directory selected by
  the user, with the file name `<profile_name>.tox`

- ![](/badge/rec.png) If the client supports user avatars, they should be stored
  under the `avatars/` directory in the root of directory selected by the user.

- ![](/badge/req.png) Avatars are named according to the following format:
  `PK.png`, where PK is the 64-character hexadecimal public key of its owner.
  Additionally, aside from avatar data, hash of an avatarshould be stored in the
  following format `PK.hash`.

- An example file heirarchy:

  ```
  +-----------------------------------------------------------------------------------+
  |   / (client working dir)                                                          |
  |    |                                                                              |
  |    +-- tox_save.tox                                                               |
  |    +-- avatars/                                                                   |
  |         |                                                                         |
  |         +-- E62DACF4C0DD23156F745874CBDBCD3D3E356F51C67921F7D91A7938CEB87933.png  |
  |         +-- E62DACF4C0DD23156F745874CBDBCD3D3E356F51C67921F7D91A7938CEB87933.hash |
  |         +-- DD2A1340FECE441206B5F3D202E6146E76617270214499B72C5511FCE839F85B.png  |
  |         +-- DD2A1340FECE441206B5F3D202E6146E76617270214499B72C5511FCE839F85B.hash |
  +-----------------------------------------------------------------------------------+
  ```
