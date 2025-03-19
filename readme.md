# Local Mirror

Get a local mirror of a web page using browser simulation. 
This is very useful for websites that render code dynamically instead of having static html.

Currently, is a half-baked mostly AI written equivalent of

```sh
wget \
--recursive \
--mirror \
--page-requisites \
--convert-links \
--no-parent \
--adjust-extension \
--span-hosts \
--wait="2" \
--random-wait \
--no-clobber \
--timestamping \
-e robots=off \
--keep-session-cookies \
--user-agent="Mozilla/5.0 (X11; Linux x86_64; rv:136.0) Gecko/20100101 Firefox/136.0" \
--load-cookies cookies.txt \
"${@}"
```

# Install

```sh
npm i -g local-mirror
```

# Usage

```sh
local-mirror <url>
```