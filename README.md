# sanstylex/sanstylex-demo

![repo size](https://img.shields.io/github/repo-size/sanstylex/sanstylex-demo.svg)
[![PyPI][pypi-badge]][pypi-link]
[![GitHub issues][issue-badge]][issue-link]
[![GitHub forks][fork-badge]][fork-link]
[![GitHub stars][star-badge]][star-link]
[![GitHub license][license-badge]][license-link]
[![contributors][contributor-badge]][contributor-link]
[![watcher][watcher-badge]][watcher-link]
[![Binder][binder-badge]][binder-link]
[![Downloads][download-badge]][download-link]
[![Documentation Status][status-badge]][status-link]
[![PyPI - Downloads][install-badge]][install-link]

学无止境！

[pypi-badge]: https://img.shields.io/pypi/v/sanstylex-demo.svg
[pypi-link]: https://pypi.org/project/sanstylex-demo/
[issue-badge]: https://img.shields.io/github/issues/sanstylex/sanstylex-demo
[issue-link]: https://github.com/sanstylex/sanstylex-demo/issues
[fork-badge]: https://img.shields.io/github/forks/sanstylex/sanstylex-demo
[fork-link]: https://github.com/sanstylex/sanstylex-demo/network
[star-badge]: https://img.shields.io/github/stars/sanstylex/sanstylex-demo
[star-link]: https://github.com/sanstylex/sanstylex-demo/stargazers
[license-badge]: https://img.shields.io/github/license/sanstylex/sanstylex-demo
[license-link]: https://github.com/sanstylex/sanstylex-demo/LICENSE
[contributor-badge]: https://img.shields.io/github/contributors/sanstylex/sanstylex-demo
[contributor-link]: https://github.com/sanstylex/sanstylex-demo/contributors
[watcher-badge]: https://img.shields.io/github/watchers/sanstylex/sanstylex-demo
[watcher-link]: https://github.com/sanstylex/sanstylex-demo/watchers
[binder-badge]: https://mybinder.org/badge_logo.svg
[binder-link]: https://mybinder.org/v2/gh/sanstylex/sanstylex-demo/main
[install-badge]: https://img.shields.io/pypi/dw/sanstylex-demo?label=pypi%20installs
[install-link]: https://pypistats.org/packages/sanstylex-demo
[status-badge]: https://readthedocs.org/projects/sanstylex-demo/badge/?version=latest
[status-link]: https://sanstylex-demo.readthedocs.io/zh/latest/?badge=latest
[download-badge]: https://pepy.tech/badge/sanstylex-demo
[download-link]: https://pepy.tech/project/sanstylex-demo

## PyPI

支持 PyPI：

```sh
pip install sanstylex/sanstylex-demo
```

## 使用

配置文档环境：

```bash
pip install .[doc]
```

构建文档：

```bash
invoke doc
```

清除文档构建：

```bash
invoke doc.clean
```

生成文档多语言翻译文件 POT (`doc/_build/gettext`)：

```bash
invoke doc.update
```

创建中文转录文件（`locales/`）：

```bash
inv doc.update -l zh_CN
```

## 其他 Sphinx 构建方法（暂时未实现）

```bash
cd doc
python -m sphinx -T -E -b readthedocssinglehtmllocalmedia -d _build/doctrees -D language=zh_CN . ../_readthedocs/htmlzip
python -m sphinx -T -E -b epub -d _build/doctrees -D language=zh_CN . ../_readthedocs/epub
```
