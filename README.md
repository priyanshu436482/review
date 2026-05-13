# Review System (Replica)

This folder contains a **local replica** of the “Business Reviews” page.

## Run locally

Because the page uses `fetch()`, you should open it through a small local server (not `file://`).

### Option A (Python)

```bash
python -m http.server 5173
```

Then open `http://localhost:5173/index.html`.

### Option B (Node)

```bash
npx serve .
```

## Notes

- The original site loads data from `api/businesses.php`.  
  This replica **tries that first**, then falls back to `mock/business.json` so it works offline.
- You can change the business id like:
  `index.html?businessId=BUS-1772092209`

