# dpu-simulator demo

An independently hosted preview of the interactive dpu-simulator website for KubeCon.

**Open the demo:** https://wizhaoredhat.github.io/dpu-simulator-demo/

The guided tour explains conventional networking, DPU offload, and the Kind/VM
simulation topology, and includes a copyable Kind quickstart.

## Source

This repository contains the generated static website. The source lives in the
`website/` directory of the dpu-simulator development checkout.

- Upstream project: https://github.com/ovn-kubernetes/dpu-simulator
- Source commit used for this publication: `4317a1cccb617438eb74cc9bb49d80adabc8ca24`
- GitHub Pages publishes `main` from the repository root.

## Update the preview

In the source checkout, from `website/`:

```sh
WEBSITE_BASE_PATH=/dpu-simulator-demo/ \
VITE_PUBLIC_URL=https://wizhaoredhat.github.io/dpu-simulator-demo/ \
npm run build
```

Copy the generated `dist/` contents into this repository, preserving `.nojekyll`,
`LICENSE`, and this README. Remove obsolete generated asset files, commit, and
push to `main`. GitHub Pages publishes the update automatically.

## Attribution

- William Zhao — Principal Software Engineer, Red Hat
- Tim Rozet — Principal Software Engineer, NVIDIA

Software is distributed under the Apache 2.0 license. Employer logos are
trademarks of their respective owners; see [asset notices](brands/NOTICE.md).
