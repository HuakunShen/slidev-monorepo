# Slidev Monorepo Template

Template for building and serving multiple slidev slides on a single website.

The template contains a website entrypoint written in vitepress in [./docs](./docs/).
You can add description and links for each slide.

## Usage

### Build

Build all slides and a vitepress entrypoint, artifact will be produced at `./dist`.

```bash
bun run build
bun run preview
```

### New Slide

```bash
cd slides
bunx create-slidev # don't install dependency, dependencies for this monorepo will be managed by bun
```

Modify the `build` script for each newly created slide like the following

```
slidev build --base /tutorial2/ --out ../../dist/tutorial2
```

