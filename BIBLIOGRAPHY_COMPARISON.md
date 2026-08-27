# Bibliography Comparison

- Previous root bibliography: 41 unique placeholder entries.
- Original ASE bibliography: 362 records representing 361 unique keys.
- Clean FSE manuscript: 27 cited keys.
- Clean FSE citations missing from the original ASE bibliography: none.
- Placeholder-only keys not present in the ASE bibliography: `euroncap2024ad` and `iso15622`. Neither is cited by the clean manuscript.

The root `references.bib` has been replaced with the original ASE bibliography entries. One duplicate-key collision was resolved without changing bibliographic content:

- `menzel_scenarios_2018`: published IEEE conference record.
- `menzel_scenarios_2018_arxiv`: arXiv version, previously stored under the same key.

The exact, unmodified supplied file is preserved at `legacy/references_ase.bib`.
