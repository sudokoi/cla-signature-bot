# Changelog

## v5.0.0 (2026-08-12)

- **Breaking**: Migrate action runtime from Node 20 to Node 24. GitHub Actions deprecated the Node 20 runtime in June 2026 and will remove it entirely in Fall 2026. This version declares `using: node24` and continues to ship the same bundled JS (compatible with both Node 20 and Node 24 runtimes).

## v4.0.0

Forked from [MetaMask/cla-signature-bot@v4.0.0](https://github.com/MetaMask/cla-signature-bot), which was itself a fork of [Roblox/cla-signature-bot](https://github.com/Roblox/cla-signature-bot).

MetaMask's improvements over the Roblox original:

- Added `allow-organization-members` input — automatically exempts members of the repository's GitHub organization
- Renamed `whitelist` → `allowlist` (with backward-compatible alias)
- Added `signature-text` and `signature-regex` inputs for custom signing phrases
- Updated Node runtime from 12 → 20
- Fixed the `issue_comment` trigger to skip non-PR comments, eliminating noisy skipped-job entries in the Actions tab
