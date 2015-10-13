Message Formatting
------------------

- ![](/badge/req.png) A client must encode emoticons as Unicode emoji.

- ![](/badge/req.png) A receiving client will make a best-effort to display
  text exactly as it was sent, and must not transform the text in any way.
    - The above rule does not apply if malformed UTF-8 text is received. In
      this case, a client may transform the text to any extent necessary to
      make it displayable.

- ![](/badge/req.png) A sending client must not insert or remove any bytes from
  the original input.

- ![](/badge/req.png) For each line of a received message, if the line begins
  with the `>` character, the client must render that line in a different
  color.
    -Green is the recommended colour, but a client may choose whichever colour
    it wants

- ![](/badge/req.png) Sent messages must be encoded in UTF-8.
