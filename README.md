# parcel-crash

Demonstrates a crash in Parcel on MacOS and Node.js v16.16.0, probably relating to the Pnpm workspace.

To reproduce, clone this repo, install dependenies and start it:

```bash
git clone https://github.com/ashleydavis/parcel-crash.git
cd parcel-crash
pnpm install
pnpm run compile
pnpm start
```This error happens with Node.js v18.9.0.MacOS 12.5.1 and 12.4.