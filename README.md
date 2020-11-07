# HTTP STatus版 Beat Saber Overlay 用 bsdp-like-overlay

これは、拙作の[Beat Saber Overlay 改良版](https://github.com/rynan4818/beat-saber-overlay)の10/31更新以降に対応した、[DataPuller](https://github.com/kOFReadie/BSDataPuller)の[BSDP-Overlay](https://github.com/kOFReadie/BSDP-Overlay)ライクなオーバーレイ用HTML&CSSです。

![preview](https://rynan4818.github.io/bsdp-like-overlay.png)

上の参考画像は、bsdp-like_rd.html (右下表示用HTML)にbsrオプションを追加しています。

## インストール方法

1. [Beat Saber Overlay bsr,no-performanceオプション追加版](https://github.com/rynan4818/beat-saber-overlay)をインストールしてください。

2. [リリースページ](https://github.com/rynan4818/bsdp-like-overlay/releases)から最新のリリースをダウンロードします。

3. zipを解凍し、1でインストールしたBeat Saber Overlayのフォルダに上書きでコピーしてください。

4. 表示位置に合わせたhtmlファイルでOBSのソースにブラウザを追加して設定してください。

| html | 表示位置 |
----|----
| bsdp-like_ld.html | 左下に譜面情報、中央上にスコア (Default) |
| bsdp-like_lt.html | 左上に譜面情報、中央下にスコア (flipHori オプション相当) |
| bsdp-like_rd.html | 右下に譜面情報、中央上にスコア (flipVert オプション相当) |
| bsdp-like_rt.html | 右上に譜面情報、中央上にスコア (flipHori&flipVert オプション相当) |

例：左下譜面情報、中央上スコア表示
```
file:///C:/TOOL/beat-saber-overlay-bsr_no-performance/bsdp-like_ld.html?modifiers=bsr
```

## オプション

次の様なオプションがURLに設定可能です。

```
file:///C:/TOOL/beat-saber-overlay-bsr_no-performance/bsdp-like_ld?modifiers=bsr
```

### `modifiers`

複数のオプションは,(カンマ)で区切ることができます。

- `hideMapDetails`
	* 譜面情報の表示を消します。
- `hideStats`
	* スコア表示を消します。
- `scale`
	* 1080p(1920x1080)の画面で使用するために、オーバーレイを1.5倍にスケーリングします。
- `bsr`
	* bsrの検索・表示をします。
- `no-hidden`
	* 終了時に表示を消しません。

## ライセンス
本HTMLとCSSは、kOF.Readie氏が製作した[BSDP-Overlay](https://github.com/kOFReadie/BSDP-Overlay)の [overlay/index.html](https://github.com/kOFReadie/BSDP-Overlay/blob/master/overlay/index.html) と [overlay/css/preset.css](https://github.com/kOFReadie/BSDP-Overlay/blob/master/overlay/css/preset.css) を元に作成しました。
元のライセンスに従い、GPL-3.0 Licenseで公開します。
