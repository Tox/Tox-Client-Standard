Export Format
-------------

- **5.1.1** ![](/badge/req.png) The client will export files relative to a folder called
  the export folder, which must be in a location accessible to the user.

- **5.1.2** ![](/badge/rec.png) The user should be able to choose the location
  of the export folder.

- **5.1.3** ![](/badge/req.png) A Toxcore data file saved in the root of the
  export folder, with the file name `<profile_name>.tox`.

- **5.1.4** ![](/badge/req.png) If the client supports user avatars, they will be stored
  under the `avatars/` directory in the root of the export folder.

- **5.1.5** ![](/badge/req.png) Avatars are named according to the following format:
  `PK.png`, where PK is the 64-character hexadecimal public key of its owner.

- An example file hierarchy:

  ```
  +-----------------------------------------------------------------------------------+
  |   / (export folder)                                                               |
  |    |                                                                              |
  |    +-- profile_name.tox                                                           |
  |    +-- avatars/                                                                   |
  |         |                                                                         |
  |         +-- E62DACF4C0DD23156F745874CBDBCD3D3E356F51C67921F7D91A7938CEB87933.png  |
  |         +-- DD2A1340FECE441206B5F3D202E6146E76617270214499B72C5511FCE839F85B.png  |
  +-----------------------------------------------------------------------------------+
  ```
