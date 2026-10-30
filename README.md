# manica-dei releases

Public release artifacts for the private source repository
[`madoo-ai/manica-dei`](https://github.com/madoo-ai/manica-dei).

The source is private. This repository contains only release assets and
mirrors the tags produced by the private release workflow. It is the download
source for the base image and `manus-dei`'s `scripts/stage-release.sh`.

Do not treat this repository as source. Do not add application code here.

## Assets

Each release carries:

- `manica-dei-linux-x64.tar.gz` — the server binary with the UI embedded
- `manica-dei-web-ui.zip` — the raw web bundle
- `release.json` — version, kind, tarball name, and tarball sha256

`release.json` is the trust anchor. Consumers verify the tarball against it.

## Mirrored by

`manus-dei` carries `scripts/mirror-release.sh` for copying a release from the
private source into this mirror. The private release remains the producer.
