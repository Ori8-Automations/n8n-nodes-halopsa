# Changelog

## [0.1.6] — 2026-07-09

### Fixed
- Credential display name changed from `HaloPSA API` to `Better HaloPSA API`, so it no longer
  collides with n8n's built-in HaloPSA credential, which uses the same label. The internal type
  name stays `haloPsaApi`, so existing credentials and the node keep resolving.

### Added
- MIT `LICENSE` file.
- README: npm status and package positioning section; tarball install example updated to 0.1.6.

---

## [0.1.5] — 2026-07-03

### Fixed
- `addNote`: added required `outcome: "Note"` field to `POST /api/Actions` payload.
  HaloPSA rejects action creation without an outcome value; observed during live testing.

---

## [0.1.4]

- Initial public release: Ticket (Create, Get, Search, Update), Action / Note (Add Note, Get Many), Attachment (Get Many, Get with signed URL).
- Live dropdowns for ticket type, client, priority, status, agent, team, site, user.
- Per-credential OAuth2 token cache.
