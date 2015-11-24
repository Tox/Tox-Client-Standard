Message Formatting
------------------

- **3.5.1** ![](/badge/req.png) A client must encode emoticons as Unicode emoji.

- **3.5.2** ![](/badge/rec.png) If malformed UTF-8 text is received a client may transform the text to any extent necessary to make it displayable.

- **3.5.3** ![](/badge/req.png) A sending client must not insert or remove any bytes from
  the original input.

- **3.5.4** ![](/badge/req.png) Sent messages must be encoded in UTF-8.
