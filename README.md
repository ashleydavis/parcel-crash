# parcel-crash

Demonstrates a crash in Parcel on MacOS.

To reproduce, clone this repo, install dependenies and start it:

```bash
git clone https://github.com/ashleydavis/parcel-crash.git
cd parcel-crash
pnpm install
pnpm run compile
pnpm start
```

The result:

```bash
zsh: segmentation fault  pnpm start
```

This crash happens with Node.js v16.16.0 and v18.9.0.
MacOS 12.5.1 and 12.4.


## A workaround

The crash can be avoided by editing packages/host-bridge/package.json and chainging the value of "main" from "build/index.js" to "src/index.ts", but this isn't an ideal fix to the problem.