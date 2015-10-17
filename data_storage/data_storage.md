Data Storage
============

A client is allowed to store profile data internally in any format.

- **5.0.1** ![](/badge/req.png) A client must give the user the option to encrypt their
  profile data.

- **5.0.2** ![](/badge/rec.png) A client should give the user the option to decrypt
  encrypted profile data.

- **5.0.3** ![](/badge/req.png) If a client's internal storage format deviates from the
  Export format defined in [Export Format](export_format.md), it will provide
  the ability to export its data into the Export format.

- **5.0.4** ![](/badge/rec.png) A client should store its profile data in the Export
  format in the standard system location defined in the following table:

  | Platform                   | Path                                  |
  |----------------------------|---------------------------------------|
  | GNU/Linux, other Unix-like | ``~/.config/tox/``                    |
  | Windows                    | ``%APPDATA%/tox/``                    |
  | Mac OS X                   | ``~/Library/Application Support/Tox`` |

