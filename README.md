# Pet Price Dashboard

Interactive SKU & brand overlap explorer for Pet Valu, PetSmart, Chewy, and Amazon.ca.

**Live site:** https://leocolab-birchhill.github.io/PetPriceDashboard/

## Enable GitHub Pages (one-time)

1. Repo **Settings** → **Pages**
2. **Build and deployment** → Source: **Deploy from a branch**
3. Branch: **main** / **/ (root)** → Save

## Update published data

From the parent `petValueScrape` project:

```bash
python match_levels.py
python build_match_dashboard.py
cd PetPriceDashboard
git add -A && git commit -m "Update dashboard data" && git push
```

The `build_match_dashboard.py` script copies all assets into this folder automatically.
