# NZBGet

Simple docker image for NZBGet without any bloat, built on the official alpine image. NZBGet runs as user `nzbget` with `uid` and `gid` `1000` and listens on port `6789`.

## Usage

```sh
docker run --rm ghudiczius/nzbget:<VERSION> \
  -p 6789:6789 \
  -v path/to/config:/config \
  -v path/to/downloads:/downloads
```

or

```sh
docker run --rm registry.gitlab.jmk.hu/media/nzbget:<VERSION> \
  -p 6789:6789 \
  -v path/to/config:/config \
  -v path/to/downloads:/downloads
```
