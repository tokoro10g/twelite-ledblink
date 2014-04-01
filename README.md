# twelite-ledblink

TWE-LiteでLEDをチカチカさせるだけのコードです．

## ビルド

そのままEclipseのプロジェクトになっているので，Linuxの場合

```
$ cd /opt/TOCOS/TWESDK/Wks_ToCoNet
$ git clone https://github.com/tokoro10g/twelite-ledblink.git LEDBlink
```

してEclipseを起動，ワークスペースにプロジェクトをインポートしてビルドしてください．

Windowsの場合はzipファイルでダウンロードして解凍したほうが楽かもしれません．
Eclipseでの処理は同様です．

## 書き込み

TWE-LiteとPCをUARTで接続，2番ピンをLOWにした状態で起動し，jenprogで書き込みます．

Linuxの場合は

```
$ jenprog.py -t /dev/ttyUSB0 LEDBlink/Build/LEDBlink_LEDBlink_JN5164_TDBG_0_1_1.bin
```

## リンク

TWE-LiteでとりあえずLチカしてみる　-　TWE-Lite - Tokoro's Tech-Note

http://wiki.tokor.org/index.php?TWE-Lite%A4%C7%A4%C8%A4%EA%A4%A2%A4%A8%A4%BAL%A5%C1%A5%AB%A4%B7%A4%C6%A4%DF%A4%EB%A1%A1-%A1%A1TWE-Lite

## ご注意

本プロジェクトはTOCOS Wireless Engineでのみ使用可能です．
コードの全部または一部を他社製品等に流用することはライセンス上できませんのでご注意下さい．

また，本プロジェクトは東京コスモス電機さまの許諾を得て，オープンソースソフトウェアとして配布しております．
ToCoNet SDK付属コードからの複製でない部分(Tokoroが記述した部分)については，MITライセンスで配布するものとします．

以下，MITライセンス

# MIT Open Source License

Copyright 2014 Tokoro

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
