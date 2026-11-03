# VoltHawk（闪鹰）Releases & Community Hub

Official binary distribution, cryptographic build provenance verification, changelogs, and issue tracker for **VoltHawk（闪鹰）** — High-Speed Non-Custodial AI Agent Workbench for BNB Smart Chain (`.ai` Agent ID Ecosystem).

---

## Verify Downloaded Installers

Every release published to this repository is built automatically via GitHub Actions with **SLSA Build Provenance Attestations** and `SHA256SUMS.txt`.

```bash
# 1. Verify SHA-256 checksum
shasum -a 256 -c SHA256SUMS.txt

# 2. Verify GitHub cryptographic build provenance
gh attestation verify <installer-filename> --owner VoltHawk
```

## Security & Open Architecture

- **100% Non-Custodial**: Private keys, mnemonics, and `@binance/agentic-wallet` (`baw`) sessions remain strictly on your local device.
- **Auditable Core**: Vault encryption (`Argon2id + AES-256-GCM`) and wallet adapters live in [`VoltHawk/volthawk-core`](https://github.com/VoltHawk/volthawk-core).

## Feedback & Bug Reports

Found a bug or want to request a feature? Please open an [Issue](https://github.com/VoltHawk/volthawk-releases/issues/new/choose). Never paste private keys, seed phrases, or API keys in public issues.
