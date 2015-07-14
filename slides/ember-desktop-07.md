# Package it

* desktop icons in `build/icons`
* can specify optional configuration; see build options for `node-webkit-builder`

```
ember nw:package
```
* `build/app/<app name>` now has folders for each platform with the appropriate app for shipping!

## Caveat
BIG FILE SIZES (40-50 MB for simple apps) because it has to pack in webkit, node, etc.
