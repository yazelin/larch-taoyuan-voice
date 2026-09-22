# larch-taoyuan-voice

《咒泉鄉》系列視覺小說的配音音檔。這裡只放音檔，產線與劇本在
[larch-taoyuan](https://github.com/yazelin/larch-taoyuan)。

Larch 的卡片用 `voiceUrl` 指到這裡的檔案，經 jsDelivr 取用：

    https://cdn.jsdelivr.net/gh/yazelin/larch-taoyuan-voice@main/lubu/<檔名>.mp3

## 為什麼音檔不放 Larch

`/voice/generate` 是逐句的，《咒泉鄉的呂布》2134 句就是 2134 次 AI 生成。
改成一次唸很多句、配完用 whisper 對齊切回來之後，切出來的片段不是 Larch 產的，
要自己託管。切分工具是 `larch-taoyuan` 的 `lubu/split.py`。

## 目錄

| | |
|---|---|
| `lubu/` | 《咒泉鄉的呂布》，檔名是 `<卡片id>-<句號>.mp3` |

`_selftest.mp3` 是給管線用的連線測試檔，不是作品內容。

## 授權

CC BY-NC 4.0 © 林亞澤 (Yaze Lin)。配音是作品內容，不是程式碼。
