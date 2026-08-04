# Manual Entropy BIP-39

An offline and auditable BIP-39 mnemonic generator that converts manually generated physical entropy into valid 12- or 24-word recovery phrases.

The project provides two standalone HTML tools:

- **Coin Entropy Generator** — generates binary entropy from coin flips.
- **Dice Entropy Generator** — generates binary entropy from dice rolls.

Both tools run entirely inside the browser and are available in three interface languages:

- English
- Portuguese (Brazil)
- Spanish

The generated BIP-39 mnemonic always uses the standard English word list for maximum wallet compatibility.

## Overview

Manual Entropy BIP-39 is a client-side tool designed to convert physical randomness into a valid BIP-39 mnemonic phrase.

Instead of relying on a computer-generated random number, the user supplies entropy collected from physical sources such as coins or dice.

The application calculates the required SHA-256 checksum and maps the resulting bit sequence to the official English BIP-39 word list.

Supported mnemonic sizes:

- 128 bits of entropy → 12 words
- 256 bits of entropy → 24 words

## Public OpenPGP Key

The public OpenPGP certificate used to verify this project's digital signatures is available at:

https://keys.openpgp.org/vks/v1/by-fingerprint/BD018CDD76ECD82A7D0CF1743915E5B9EFAF157E

Fingerprint:

```text
BD01 8CDD 76EC D82A 7D0C F174 3915 E5B9 EFAF 157E
