[English](README.md) | 简体中文

<p align="center">
  <br>
  <a href="https://sherlockproject.xyz/" target="_blank"><img src="images/sherlock-logo.png" alt="sherlock"/></a>
  <br>
  <span>按用户名在 <a href="https://sherlockproject.xyz/sites">400+ 个社交网络</a>中追查社交媒体账号</span>
  <br>
</p>

<p align="center">
  <a href="https://sherlockproject.xyz/installation">安装</a>
  &nbsp;&nbsp;&nbsp;•&nbsp;&nbsp;&nbsp;
  <a href="https://sherlockproject.xyz/usage">用法</a>
  &nbsp;&nbsp;&nbsp;•&nbsp;&nbsp;&nbsp;
  <a href="https://sherlockproject.xyz/contribute">贡献</a>
</p>

<p align="center">
<img width="70%" height="70%" src="images/demo.png" alt="演示"/>
</p>


## 安装

<div align="center">
  <a href="https://sponsors.sherlockproject.xyz/go/readme-1"><img src="https://sponsors.sherlockproject.xyz/banner/readme-1" width="100%"></a>
</div>

<div align="center">
<a href="https://sponsors.sherlockproject.xyz/go/readme-2"><img src="https://sponsors.sherlockproject.xyz/banner/readme-2" width="49.8%"></a>&#8202;&#8202;<a href="https://sponsors.sherlockproject.xyz/go/readme-3"><img src="https://sponsors.sherlockproject.xyz/banner/readme-3" width="49.8%"></a>
</div>

<br>

> [!WARNING]  
> 由第三方维护的 ParrotOS 与 Ubuntu 24.04 软件包似乎已经__无法使用__。  
> 这些系统的用户应改用 [`uv`](https://docs.astral.sh/uv/)/`pipx`/`pip` 或 Docker。

| 方式 | 说明 |
| - | - |
| `pipx install sherlock-project` | 可用 `pip` 或 [`uv`](https://docs.astral.sh/uv/) 代替 `pipx` |
| `docker run -it --rm sherlock/sherlock` |
| `dnf install sherlock-project` | |

社区维护的软件包可用于 Debian（>= 13）、Ubuntu（>= 22.10）、Homebrew、Kali 和 BlackArch。这些软件包并非由 Sherlock Project 直接支持或维护。

请在[这里](https://sherlockproject.xyz/installation)查看全部替代安装方式。

## 常规用法

只搜索一个用户：
```bash
sherlock user123
```

搜索多个用户：
```bash
sherlock user1 user2 user3
```

找到的账号将保存到以对应用户名命名的单独文本文件中（例如 ```user123.txt```）。

```console
$ sherlock --help
usage: sherlock [-h] [--version] [--verbose] [--folderoutput FOLDEROUTPUT] [--output OUTPUT] [--csv] [--xlsx] [--site SITE_NAME] [--proxy PROXY_URL] [--dump-response]
                [--json JSON_FILE] [--timeout TIMEOUT] [--print-all] [--print-found] [--no-color] [--browse] [--local] [--nsfw] [--txt] [--ignore-exclusions]
                USERNAMES [USERNAMES ...]

Sherlock: Find Usernames Across Social Networks (Version 0.16.0)

positional arguments:
  USERNAMES             One or more usernames to check with social networks. Check similar usernames using {?} (replace to '_', '-', '.').

options:
  -h, --help            show this help message and exit
  --version             Display version information and dependencies.
  --verbose, -v, -d, --debug
                        Display extra debugging information and metrics.
  --folderoutput FOLDEROUTPUT, -fo FOLDEROUTPUT
                        If using multiple usernames, the output of the results will be saved to this folder.
  --output OUTPUT, -o OUTPUT
                        If using single username, the output of the result will be saved to this file.
  --csv                 Create Comma-Separated Values (CSV) File.
  --xlsx                Create the standard file for the modern Microsoft Excel spreadsheet (xlsx).
  --site SITE_NAME      Limit analysis to just the listed sites. Add multiple options to specify more than one site.
  --proxy PROXY_URL, -p PROXY_URL
                        Make requests over a proxy. e.g. socks5://127.0.0.1:1080
  --dump-response       Dump the HTTP response to stdout for targeted debugging.
  --json JSON_FILE, -j JSON_FILE
                        Load data from a JSON file or an online, valid, JSON file. Upstream PR numbers also accepted.
  --timeout TIMEOUT     Time (in seconds) to wait for response to requests (Default: 60)
  --print-all           Output sites where the username was not found.
  --print-found         Output sites where the username was found (also if exported as file).
  --no-color            Don't color terminal output
  --browse, -b          Browse to all results on default browser.
  --local, -l           Force the use of the local data.json file.
  --nsfw                Include checking of NSFW sites from default list.
  --txt                 Enable creation of a txt file
  --ignore-exclusions   Ignore upstream exclusions (may return more false positives)
```

## 致谢

感谢每一位为 Sherlock 做出贡献的人！❤️

<a href="https://github.com/sherlock-project/sherlock/graphs/contributors">
  <img src="https://contrib.rocks/image?&columns=25&max=10000&&repo=sherlock-project/sherlock" alt="贡献者"/>
</a>

## 星标历史

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=sherlock-project/sherlock&type=Date&theme=dark" />
  <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=sherlock-project/sherlock&type=Date" />
  <img alt="Sherlock Project 星标历史图" src="https://api.star-history.com/svg?repos=sherlock-project/sherlock&type=Date" />
</picture>

## 许可证

MIT © Sherlock Project<br/>
创建者 - [Siddharth Dushantha](https://github.com/sdushantha)

<!-- Reference Links -->

[ext_pypi]: https://pypi.org/project/sherlock-project/
[ext_brew]: https://formulae.brew.sh/formula/sherlock
