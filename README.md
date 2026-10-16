# miyu-memes-shorin-collection

给 Miyu 的「表情包」软件包（[miyu-agent/miyu-memes](https://github.com/miyu-agent/miyu-memes)）带的一套图：旧版 Miyu 的 38 张，描述、用法照旧。没有程序，只有清单和 `memes/`。

```sh
miyu pkg install ./miyu-memes-shorin-collection
```

装上以后表情包会把这些图读进库（来源记「内容包」）；卸了，没被人改过的那些一起拿掉。

- `package.toml`：`[content.miyu-memes] dir = "memes"`。
- `memes/index.json`：`{"memes": [{"file", "description", "usage"}]}`，别的格不读。
- `memes/images/`：图。
