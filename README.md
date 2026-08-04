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

## Included Tools

The repository contains two independent HTML files.

### Coin Entropy Generator

This version accepts results obtained from repeated coin flips.

Each result represents one binary bit:

```text
Heads → 1
Tails → 0
