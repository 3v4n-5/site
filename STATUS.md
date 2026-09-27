# Status — 2026-09-27

## Done (live on 3v4n.netlify.app, site `041c7ef`)
- Removed BROKE.001/002 posts and the dead `soundcloud.com/sys_ex` link (`links.ts`, `GlobalFx.tsx`).
- `audio/releases/test_001`: embed of `soundcloud.com/thr33v33/test_001`, no text.
- `projects/systems/usage-ring`: post for `github.com/3v4n-5/usage-ring` (public, source only). `Projects/usage-ring` in the vault is now a submodule of it. No screenshot yet.
- `projects/visuals/vidgen`: post with 5 clips in `public/videos/vidgen/`, from `VidGen/outputs/vids/sweeps/sweep{1,2}`. Reuses `imgen.ref.mdx`; `vidgen.prompts.mdx` samples `VidGen/prompts.md`.

## Open
- Second VidGen video: add when finished.
- `imgen.mdx` "Next steps" still says video is next; could link `vidgen`.
- `about-me.mdx` links `github.com/n4m3name` (404; account is now `3v4n-5`). `necrotype.mdx` and `dotfiles.mdx` use the same name; those redirect.
- usage-ring post: add a menu-bar screenshot.
- Uncommitted, not from this session: `content/research/statistics/ahabs-harpoon.mdx`, `public/images/eJAB/flow_chart.svg`, `public/images/eJAB/flow_chart.dot`.
- The Air: `cd ~/Notes && rm -rf Projects/usage-ring/.build && git submodule update --init Projects/usage-ring && dev-sync pull Projects/Site`

## Notes
- `pnpm build` fails on pnpm's build-script approval (`pnpm approve-builds`). Build with `./node_modules/.bin/tsc -b && ./node_modules/.bin/vite build`.
- The site renders no Markdown tables (no remark-gfm); use lists.
- `dev-sync push` refuses while the files above are uncommitted: `git stash push -u`, push, `git stash pop`.
