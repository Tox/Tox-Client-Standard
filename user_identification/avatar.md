Avatar
------

- ![](/badge/rec.png) A Tox client should allow the user to provide an image
  representation of themselves to be sent to friends.

- ![](/badge/req.png) If a Tox client does not support avatars, all received
  file transfers of the type `TOX_FILE_KIND_AVATAR` must be cancelled
  immediately.

Avatar support in Tox clients is not required. The points below are applicable only to clients that provide avatar support.

- ![](/badge/req.png) Avatars must be PNG images.

- ![](/badge/req.png) The maximum size of the encoded avatar data is 65536
  bytes (64KiB).

- ![](/badge/req.png) The user must be allowed to unset the avatar.

- ![](/badge/req.png) When a friend comes online, and an avatar is set, the
  client will send a file transfer of type `TOX_FILE_KIND_AVATAR`, where the
  file ID is the hash of the avatar data that will be sent.

- ![](/badge/req.png) When a user sets a new avatar, the client will send a
  file transfer of type `TOX_FILE_KIND_AVATAR` to all friends, where the file
  ID is the hash of the avatar data that will be sent.

- ![](/badge/req.png) When a user unsets an avatar, the client will send an
  avatar file transfer of size 0 to all friends. In this case, the file ID is
  undefined.

- ![](/badge/req.png) When a file transfer of type `TOX_FILE_KIND_AVATAR` is received:
    - The client must check the file ID against a previously-saved hash of the
      friend's avatar. If it is the same, the client must cancel the transfer,
      and use the previously-stored avatar.
    - The client must check the file size against the maximum size. If it is
      greater, the transfer must be cancelled.
    - If the file size is 0, the transfer must be cancelled, and any cached
      avatar data for that friend must be purged.
    - If the transfer does not meet any of the conditions for cancellation, the
      avatar must be saved and displayed, and the hash of the file must be
      stored alongside the avatar itself.
    - The client must keep at least one unmodified copy of the avatar on disk.
      Any modificaion for display purposes must be done only in memory, or in a
      temporary file.
