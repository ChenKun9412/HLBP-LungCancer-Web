# HLBP LungCancer Web

This directory is the public web bundle exported from the private analysis repo.

Contents:
- `site/index.html`: static website entrypoint
- `site/.nojekyll`: disables Jekyll processing on GitHub Pages

Recommended usage:
1. Create a separate public repository, for example `HLBP-LungCancer-Web`
2. Copy everything under `site/` into that public repository
3. Enable GitHub Pages on the public repository

After each update in the main repo, regenerate this bundle with:

```bash
/home/chenkun/miniconda3/envs/hlbp/bin/python build_airway_feature_dashboard.py
python export_web_release.py
```
