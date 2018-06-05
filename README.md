我的鼠鬚管輸入法配置
================
 輸入方案使用小鶴雙拼，擴充了[詞庫](https://github.com/rime-aca/dictionaries)添加了[小鶴音形](https://github.com/nunchaju/rime-hepy)輸入方案，利用反查（[reverse_lookup](https://github.com/Aben/squirrel-setting/blob/d218c8baf7f62bce91fa53293ff5656dc23ceb27/double_pinyin_flypy.custom.yaml#L10)）輸入生僻字，不用翻頁去查找，代價就是需要學習形碼，製作了一份「batman」的皮膚，順便折騰了一下字體，需要自行安裝字體。

安装
------
因爲鼠鬚管好久沒發佈更新包了，所以我自己編譯了一份，玩法有了一些變化，不折騰不舒服斯基：）

第一步，自己編譯一份最新版的[鼠鬚管](https://github.com/rime/squirrel)，官方教程

[https://github.com/rime/squirrel/blob/master/INSTALL.md](https://github.com/rime/squirrel/blob/master/INSTALL.md)

第二步，安裝[東風破 /plum/](https://github.com/rime/plum)，新玩法。

```shell
cd ~//Library/Rime
curl -fsSL https://git.io/rime-install | bash
./plum/rime-install prelude essay luna-pinyin double-pinyin emoji
```

第三步，複製文件，根據自己的需求做適當修改定製文件配置`*.custom.yaml`，有註釋。

```shell
cd ~/Workspace
git clone https://github.com/Aben/squirrel-setting.git
cp *.yaml ~/Library/Rime/
```

注意：

* `installation.yaml`添加sync_dir可修改備份目錄，比如備份到iCloud。

```yml
sync_dir: "/Users/<User>/Library/Mobile Documents/com~apple~CloudDocs/RimeSync"
```

ChangeLog
------
1. 擴充了[詞庫](https://github.com/rime-aca/dictionaries)
2. 添加了[小鶴音形](https://github.com/nunchaju/rime-hepy)輸入方案
3. 製作了一份「batman」的皮膚。

*****
憑記憶整理的，有遺漏或錯誤提issue吧


