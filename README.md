# Crosschain Interoperability WG: group page

**This repo is the live site.** GitHub Pages serves `docs/` at
<https://entethalliance.github.io/crosschain-interoperability/>; the historical
`entethalliance.org/groups/crosschain/` URL 301-redirects here (WP Engine rule,
applied by Redwan).

Built per the
[WG Modernization Playbook](https://github.com/EntEthAlliance/eea-design-system/blob/main/WG_MODERNIZATION_PLAYBOOK.md)
on the EEA design system **editorial family**. Reference sibling:
[wg-ethtrust-site](https://github.com/EntEthAlliance/wg-ethtrust-site).

## Layout

- `docs/index.html`: the WG page (content parity with the previous
  /groups/crosschain/ page: focus, publications, videos, blog, chairs,
  contribute, contact).
- `docs/*.html`: content-identical restyled copies of the WG's documents
  (Crosschain ID spec, Security + Decentralization Guidelines, DLT interop
  technical-spec editor's draft) at their **original filenames**, so
  pre-rename links to `…/crosschain-interoperability/<doc>.html` resolve
  again. Canonicals point at the `wg-crosschain` Pages originals. CRLF
  sources are normalized to LF; otherwise one stylesheet link + return bar
  added, nothing else.
- `docs/og-card.png`, `robots.txt`, `sitemap.xml`: SEO layer; shared EEA
  Pages Google tag on all pages.

## Deploying

Merge a PR to `main`: Pages redeploys. No WordPress step; rollback of the
redirect = delete the rule in the WP Engine portal (old files untouched).

## History

The WG's repo was renamed `crosschain-interoperability` → `wg-crosschain`,
which silently broke the old GitHub Pages URL (Pages does not redirect
renames): including links from the WG's own draft-merge stubs. This repo
restores that URL as the WG's public home. The `wg-crosschain` repo remains
the working repo for specs and meeting material.
