WhatsAPINet
===========

This is a API written in C# but it can be used in any .NET language. It's a fork from WhatsAPINet, which is based on WhatsAPI.
The goal of this fork is to make it all work again and refacter the code, add documentation and write documentation
on how Whatsapp works.

## Protocol
The WhatsApp protocol is sadly not officially documented. While working on this
project, I will try to document most of my progress in the docs folder.

The protocol is based on the XML-based XMPP protocol, a heavily documented
internet messaging protocol. To reduce the XML overhead, the XML structure and a
lot of common keywords are converted into bytes. See docs/funxmpp.txt for a
more detailed explanation. Sadly, the XMPP standard is not followed exactly
everywhere.

* Protocol wrapper: FunXMPP (see doc/funxmpp.txt)
* Main protocol: XMPP (http://xmpp.org/rfcs/rfc6120.html)
* Authentification: SASL, digest auth (http://tools.ietf.org/html/rfc2831)
* Blocking: XMPP privacy lists? (http://xmpp.org/extensions/xep-0016.html)
* Ping (http://xmpp.org/extensions/xep-0199.html)
