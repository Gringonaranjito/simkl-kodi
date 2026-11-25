# Release plan

Status: private staging; no live Kodi update feed yet.

## Tested baseline
- Simkl 0.9.29: S21 movie playback and restart tested by owner.
- context.simkl 1.0.35.
- Elementum 0.1.119.1: Android ARM64 on-demand test build. Do not publish this binary as a universal Kodi update.

## Distribution
- Update feed: platform-independent Simkl and context.simkl only, using Kodi addons.xml and checksum plus standard per-addon ZIP paths.
- Full installation: separate architecture-specific offline bundles. Android ARM64 bundle exists; Windows and other Android architectures need their own validation.
- Keep Elementum automatic updates disabled until a safe architecture-aware distribution is tested.
- Preserve userdata and account authorization; never commit Kodi backups, logs or personal settings.
- Retain original licenses and attribution. Review upstream application credentials and redistribution terms before public hosting.
- Test the feed and installation on a spare Kodi profile before enabling automatic updates on the working S21.
