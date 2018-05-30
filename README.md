我的鼠鬚管輸入法配置
================
 輸入方案使用小鶴雙拼，擴充了[詞庫](https://github.com/rime-aca/dictionaries)，添加了[小鶴雙拼形碼](https://github.com/zecy/flypy_double)輸入方案，準備嘗試一下，製作了一份「batman」的皮膚，顺带折腾了一下字体。

安装
------
因爲鼠鬚管好久沒發佈更新包了，所以我自己編譯了一份，玩法有了一些變化，不折騰不舒服斯基：）

第一步，自己編譯一份最新版的[鼠鬚管](https://github.com/rime/squirrel)，官方教程

[https://github.com/rime/squirrel/blob/master/INSTALL.md](https://github.com/rime/squirrel/blob/master/INSTALL.md)

第二步，安裝[東風破 /plum/](https://github.com/rime/plum)，新玩法。

```shell
cd ~//Library/Rime
curl -fsSL https://git.io/rime-install | bash
./plum/rime-install prelude luna-pinyin double-pinyin emoji
```

第三步，複製文件，根據自己的需求做適當修改定製文件配置`*.custom.yaml`，有註釋。

```shell
cd ~/Workspace
git clone https://github.com/Aben/squirrel-setting.git
cp *.yaml ~/Library/Rime/
```

注意：

* `double_pinyin_flypy.custom.yaml` 適用於所有雙拼方案（「自然碼雙拼」、「智能ABC雙拼」、「小鶴雙拼」、「MSPY雙拼」）。只須將此`custom.yaml` 的前面名字改爲對應的輸入方案名字然後放入用戶文件夾重新部署即可。如 `double_pinyin_abc.custom.yaml`。

* `installation.yaml`添加sync_dir可修改備份目錄，比如備份到iCloud。

```yml
sync_dir: "/Users/<User>/Library/Mobile Documents/com~apple~CloudDocs/RimeSync"
```

ChangeLog
------
1. 擴充了[詞庫](https://github.com/rime-aca/dictionaries)
2. 添加了[小鶴雙拼形碼](https://github.com/zecy/flypy_double)輸入方案（試驗階段）
3. 製作了一份「batman」的皮膚。

*****
憑記憶整理的，有遺漏或錯誤提issue吧


