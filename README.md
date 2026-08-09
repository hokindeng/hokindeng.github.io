# hokindeng.github.io — redirect only

The personal site moved to **https://hokindeng.com/** on 2026-08-08.
It is now served from EC2; this repo only redirects there.

- `index.html` — redirects to `https://hokindeng.com/`
- `404.html` — redirects and carries the path over, so old deep links
  (`/share/`, `/index_andy.html`, `/images/...`) still land on the right page

**The site content now lives in `hippocampal-company/hokindeng-web` under `site/`.**
Edit it there — changes deployed to the box are what hokindeng.com serves.

Note: a `CNAME` file must NOT be added here. That would make GitHub Pages claim
`hokindeng.com` and require its DNS to point at GitHub, which would break the
EC2 hosting. The redirect above is client-side because Pages cannot issue a 301.

The previous site is still in this repo's git history (before the 2026-08-08
redirect commit) if it is ever needed.
