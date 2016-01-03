Message Formatting
------------------

- **3.5.1** ![](/badge/req.png) A client must encode emoticons as Unicode emoji.

- **3.5.2** ![](/badge/req.png) A receiving client will make a best-effort to display
  text exactly as it was intended, and must not materially change the text in any way.
    - The above rule does not apply if malformed UTF-8 text is received. In
      this case, a client may transform the text to any extent necessary to
      make it displayable.

- **5.3.3** ![](/badge/rec.png) It's a strong suggestion that messaging clients support 
  at the very least a subset of the common markdown syntax. The markdown used in this 
  standard is a subset of Github Flavored Markdown. With the exclusion of direct 
  links/referneces.
    - ![](/badge/req.png) If the client implments any kind of markdown support, it must 
      not conflict in any way with the markdown used in this standard.
    - This Flavor of markdown was chosen because of it's protection of common code syntax.
    - Clients are free to implement any subset or different markdown or markdown like syntax
      given it doesn't conflict with this standard.

- **3.5.4** ![](/badge/req.png) A sending client must not insert or remove any content/data
  from any message, of any type. Clients may trim white space from a text messages with the
  exception of newline and carrage returns, they must not be altered in anyway.

- **3.5.5** ![](/badge/req.png) Sent messages must be strictly compatable with UTF-8.
