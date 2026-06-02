# Janklar

Janklar is a lightweight, sovereign encryption engine designed for high-integrity data transit in resource-constrained environments. It provides a zero-trust approach to data masking, specifically engineered to operate on low-spec hardware without reliance on centralized key management.

## Core Features
- **Sovereign Engine:** Bitwise-based cryptographic operations optimized for minimal memory footprint.
- **Offline-First:** Designed to function in air-gapped environments.
- **Integrity Verification:** Includes a MAC-based verification layer to ensure data has not been tampered with in transit.
- **Abelwrap CLI:** A specialized command-line interface for seamless encryption/decryption of trade and sensitive documents.

## Why Janklar?
Standard encryption tools often require significant overhead and persistent connectivity, which are not viable in low-budget, high-threat scenarios. Janklar bridges this gap, offering a resilient alternative for individual sovereignty.

## Usage
The system utilizes the `./sovereign` binary for data processing:

```bash
# Encrypt a file
./sovereign -e <input_file> <output_file>

# Decrypt a file
./sovereign -d <locked_file> <output_file>
