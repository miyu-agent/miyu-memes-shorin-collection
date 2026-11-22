<p align="center">
  <a href="README.md">English</a> | 简体中文
</p>

# 表情包合集（memes-shorin-collection）

> <sub>本文档由 Anthropic 的 Claude Fable 5.2 生成。</sub>

这是给 Miyu 的「表情包」软件包（[miyu-agent/miyu-memes](https://github.com/miyu-agent/miyu-memes)）准备的一套图片：一共 38 张，来自旧版 Miyu，图片的描述和用法仍然沿用旧版。这个软件包没有程序，只有清单和 `memes/` 目录。

运行以下命令安装：

```sh
miyu pkg install memes-shorin-collection
```

如果要从源码安装，把这个仓库克隆成名叫 `memes-shorin-collection` 的文件夹（文件夹名就是软件包编号），再运行 `miyu pkg install ./memes-shorin-collection`。

安装以后，「表情包」软件包会把这些图片读进图库（来源记为「内容包」）；卸载这个软件包时，没有被人修改过的图片会一起被移除。仓库里的文件如下：

- `package.toml`：`[content.memes] dir = "memes"`（这个软件包的编号是 `memes-shorin-collection`，它为编号是 `memes` 的「表情包」软件包提供内容）。
- `memes/index.json`：`{"memes": [{"file", "description", "usage"}]}`，其他字段不会被读取。
- `memes/images/`：图片。
