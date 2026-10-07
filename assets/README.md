# Profile artwork

Original, self-contained SVG artwork for the Scorpascal profile.

- `hero-dark.svg` / `hero-light.svg`: theme-specific orbital constellation banners.
- `project-*.svg`: illustrated project headers, with no live metrics or research details.
- `workflow.svg`: decorative question/build/verify/refine loop, not a progress indicator.
- `divider.svg`: gradient separator with a slow traveling highlight.
- `stack-*.svg`: text-based technology badges; abbreviations are not official product logos.

The README uses image references rather than inline SVG or page scripts. All artwork is stored in this repository, with no external fonts, trackers, scheduled jobs, or image-generation services needed at runtime. The README selects each animated SVG's `#still` fragment under `prefers-reduced-motion: reduce`, and the SVG also includes a reduced-motion CSS rule. The fragment explicitly disables animations while retaining the same artwork, including in image contexts that do not inherit the media preference. Clients that do not play SVG animation can still display the base illustration. Theme selection is handled with the README's `picture` sources.

To adjust the visual identity, edit the SVG text, color values, and animation durations. Keep titles, descriptions, and README image alternatives accurate. Do not put private research data, progress counters, unpublished results, or credentials in these public assets.
