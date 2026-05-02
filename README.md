# Longbridge Pro (Flatpak)

Flatpak packaging for [Longbridge Pro](https://longbridge.com/desktop/), a
professional securities trading desktop application.

The upstream binary is repackaged from the Debian release published at
<https://assets.lbkrs.com/github/release/longbridge-desktop/stable/>.
Releases are tracked automatically via `x-checker-data` against
`latest.json`.

## Bundled fonts

Longbridge's GUI does not pick up the fonts shipped by the GNOME
runtime and panics at startup when it cannot resolve one of the font
families it knows about. To keep the application usable out of the
box, two Noto fonts (Regular weight only) are installed into
`/app/share/fonts/`:

- **Noto Sans Regular** — Latin/Greek/Cyrillic coverage, sourced from
  [`notofonts/notofonts.github.io`](https://github.com/notofonts/notofonts.github.io)
  (`noto-monthly-release-2026.05.01`).
- **Noto Sans CJK Regular** — CJK coverage, sourced from
  [`notofonts/noto-cjk`](https://github.com/notofonts/noto-cjk)
  (`Sans2.004`).

Both fonts are licensed under the
[SIL Open Font License 1.1](https://scripts.sil.org/OFL); the license
texts are bundled next to the font files as
`NotoSans.LICENSE.txt` and `NotoSansCJK.LICENSE.txt`.
