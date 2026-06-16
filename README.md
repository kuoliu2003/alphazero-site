# AlphaZero explainer — website

Source for the public AlphaZero explainer page, hosted on Cloudflare Pages at
**https://alphazero.kuosmindpalace.com**.

This repo is intentionally tiny — just the deployable site:

```
index.html        the explainer (self-contained: inline CSS/SVG, MathJax/fonts via CDN)
results/*.png     the four result figures the page embeds
```

It's a static site — no build step. Cloudflare Pages serves `index.html` at the
root; every push to `main` redeploys automatically.

## Updating the page

Edit `index.html` (or drop in updated figures) and push to `main`. Cloudflare
Pages rebuilds within ~a minute.

## Where the rest lives

The full project — the Julia/AlphaZero.jl training and benchmark code, all data
and source CSVs, the model weights, and the interactive play app — is in the
private project repo **`alphazero-go9`**. This website repo only holds what is
published.

## Local preview

```
python -m http.server 8000      # then open http://127.0.0.1:8000
```
