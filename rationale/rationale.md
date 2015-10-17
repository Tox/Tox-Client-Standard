Rationale
============

The purpose of the rationale is to expound on clauses for which the purpose may be confusing or unobvious. The criteria for including a clause in this document is somewhat arbitrary; inclusion is decided on a case to case basis, usually in response to questions or confusion within the Tox development community.

- **1.0.2** If a user's client is configured to use a proxy, it is reasonable to assume that they may be doing so in order to mask their IP address. Therefore users must be made aware that UDP traffic may bypass the proxy and reveal their IP address.

- **1.0.3** If a user's client is configured to use a proxy with UDP connections disabled, it must be assumed that the user's intent is to mask their IP address. Therefore it should not be possible to bypass the proxy.

- **1.0.4** Third party services cannot be accounted for by the Tox project and are contrary to the decentralized nature of Tox. They may be unreliable, insecure or otherwise compromised. Therefore the user should always have the option to use the client in a fully functional manner (in relation to the functionality made available via the Tox API) without being forced to use third party services.

- **2.2.2** This is to account for colour blindness in respect to the fact that the recommended user status colours are not colour-blind friendly.

- **2.3.3** PNG images are currently the only image type supported by Tox avatars.

- **2.3.8** This will ensure that the avatar is unset for all of the user's friends (as long as their clients comply with clause 2.3.9).

- **3.1.2** When a friend request is accepted, certain identifying information may become available to initiator of the request. In respect to protecting user privacy, this must not occur without a user's explicit consent.

- **3.1.3** This provides a way for users to verify the identity of the requestor out of band (e.g. over the phone or in person) before accepting the request.

- **3.2.2** When a user joins a group, certain identifying information may become available to all peers in the group. See also: 3.1.2.

- **3.2.3** A peer's identity in a group, which includes their group public key and role/permissions, is persistent across client restarts. However this identity is permanently lost when the client explicitly leaves the group.

- **4.0.2** As message history may be stored on a user's device in plaintext, it is a matter of security to ensure that this does not occur without the user's explicit consent.
