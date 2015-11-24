Message Formatting
------------------

- **3.5.1** ![](/badge/req.png) A client must encode emoticons as Unicode emoji.

- **3.5.2** ![](/badge/req.png) A receiving client will make a best-effort to display
  text exactly as it was sent, and must not transform the text in any way.
    - The above rule does not apply if malformed UTF-8 text is received. In
      this case, a client may transform the text to any extent necessary to
      make it displayable.

- **3.5.3** ![](/badge/req.png) A sending client must not insert or remove any bytes from
  the original input.

- **3.5.4** ![](/badge/req.png) Sent messages must be encoded in UTF-8.
