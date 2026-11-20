# sidechic

brainrot ad agency landing page. static HTML, no build step. site lives in `public/`.

## deploy (Cloudflare Workers, static assets)

Config is in `wrangler.jsonc` (Worker name `sidechic`, serves `./public`).

- CLI: `npx wrangler@4 deploy`
- Or Cloudflare dashboard → Workers & Pages → Create → Import a repository → pick this repo (deploy command `npx wrangler deploy`, no build command).

Custom domain: Workers & Pages → `sidechic` → Settings → Domains & Routes → Add → Custom domain.

## local preview

```
npx serve public
```
