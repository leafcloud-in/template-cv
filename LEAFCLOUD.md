# LeafCloud adaptation

- Upstream: https://github.com/BartoszJarocki/cv
- Author: Bartosz Jarocki
- Licence: MIT (upstream LICENSE retained unchanged)
- Pinned upstream commit: dad4e4b27190cfaa83c9f5e0a2f8a54d60ba3323
- Preview: https://tpl-cv.leafcloud.app (not live: LeafCloud site limit)

Adaptation: added LeafCloud setup guidance, fictionalized visible author/demo identity where found, and configured static output where required. Original visual design retained.

Static export fixes: set `output: "export"`, `images.unoptimized`, and `dynamic = "force-static"` on the metadata routes. Removed unsupported custom headers and replaced the upstream portrait with a fictional initials graphic. `pnpm run build` passes.

pnpm 11.11.0 compatibility: pinned `packageManager`, set `minimumReleaseAge: 0` while retaining the required Next.js release-age exclusions, and approved the `esbuild` and `sharp` install scripts in `pnpm-workspace.yaml`.
