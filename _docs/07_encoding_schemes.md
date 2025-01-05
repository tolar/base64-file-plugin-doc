---
title: Encoding Schemes
layout: single
collection: docs
toc: false
weight: 7
permalink: /encoding_schemes
---

The plugin supports three Base64 encoding schemes: ***BASIC***, ***MIME***, and ***URL and Filename Safe***.
These schemes are based on the standards defined in [RFC 4648](https://www.ietf.org/rfc/rfc4648.txt)
and [RFC 2045](https://www.ietf.org/rfc/rfc2045.txt).

By default, the plugin uses the MIME scheme for encoding and decoding files. 
Users can change the encoding scheme of an encoded file through the appropriate action in the editor's popup menu. 
See [Encoded File Actions](http://127.0.0.1:4000/editor#encoded-file-actions) for details.

| Scheme | Definition                                                                                                                                                  | Key Characteristics                                                                                                                                                                                                                                                                                                                                                    |
|--------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| BASIC  | Uses "The Base64 Alphabet" as specified in Table 1 of [RFC 4648](https://www.ietf.org/rfc/rfc4648.txt) and [RFC 2045](https://www.ietf.org/rfc/rfc2045.txt) | Does not add any line feed (line separator) characters to the encoded output.<br/><br/>Rejects data containing characters outside the Base64 alphabet during decoding.                                                                                                                                                                                                 |
| URL    | Uses the "URL and Filename Safe Base64 Alphabet" as specified in Table 2 of [RFC 4648](https://www.ietf.org/rfc/rfc4648.txt).                               | Replaces <kbd>+</kbd> with <kbd>-</kbd> and <kbd>/</kbd> with <kbd>_</kbd> in the encoded output to ensure compatibility with URLs and filenames.<br/><br/>Does not add any line feed (line separator) characters to the encoded output.<br/><br/>Rejects data containing characters outside the Base64 alphabet during decoding.                                      |
| MIME   | Uses "The Base64 Alphabet" as specified in Table 1 of [RFC 2045](https://www.ietf.org/rfc/rfc2045.txt).                                                     | Encoded output is formatted in lines of no more than 76 characters.<br/><br/>Uses a carriage return (<kbd>\r</kbd>) followed by a linefeed (<kbd>\n</kbd>) as the line separator.<br/><br/> Does not add a line separator at the end of the encoded output.<br/><br/>Ignores all line separators or other characters not found in the Base64 alphabet during decoding. |

