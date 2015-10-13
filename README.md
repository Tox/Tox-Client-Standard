Introduction
============

- This document is intended to define behaviours that are not enforced by
  toxcore, but are otherwise required/recommended to ensure proper client
  interoperability as well as best security practices.

- For a Tox client to be endorsed/supported (?) by the Tox project, it must, at
  minimum, comply with every ![](badge/req.png) point in this document (except
  where otherwise stated).  For this reason, things that are ![](badge/req.png)
  should not be needlessly specific.
    - For example, this is a **bad** ![](badge/req.png) point: *A Tox client
      will show a message timestamp in the format HH:MM:SS, to the left of each
      message, with 10 pixels of whitespace between.*
    - A better point would be: *A Tox client will allow users to see when a
      message was received.*

- Sometimes, it is not immediately obvious why certain points exist in this
  document. For this purpose, there is a Rationale section, where explanations
  will be given.
