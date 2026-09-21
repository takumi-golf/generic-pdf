<div align="center">

# ジェネリックPDF / Generic PDF

**有名な PDF 編集サービスと同じ効能を、添加物なしで。**
**The same effects as the big-name PDF editors, with no additives.**

文字入れ・押印・手書き署名・結合・分割・回転・トリミング・透かし・ページ番号・フォーム記入・パスワード・墨消し・画像変換・圧縮。
**ファイルはあなたの PC から出ません。** 会員登録もカード登録もなし、0 円、HTML 1 ファイル。

Add text, stamps and hand-drawn signatures. Merge, split, rotate, crop. Watermarks, page numbers, form filling, passwords, redaction, image conversion, compression.
**Your files never leave your computer.** No account, no credit card, free, one HTML file.

[**いますぐ使う / Use it now → https://ilove-ai.net/pdf**](https://ilove-ai.net/pdf)　·　[ダウンロード版 / Download → Releases](../../releases)

日本語 / English（画面右上で切替 / toggle in the top-right corner）

</div>

---

## なぜこれか / Why

PDF を少し直したいだけなのに、先発品は月額課金、無料の Web サービスはファイルをサーバーに送ります。
このツールは **ブラウザの中だけで** 処理します。`index.html` を読めば、ファイル本体を送る `fetch` / `XMLHttpRequest` が
**存在しない**ことを確認できます。ネットワークに出るのはライブラリとフォントの取得だけです。

You just want to touch up a PDF, but the big names charge a subscription and the free web tools upload your file to a server.
This tool does everything **inside the browser**. Read `index.html` and you will find **no** `fetch` / `XMLHttpRequest` that sends
your file anywhere. The only network requests fetch libraries and fonts.

- アップロードしない / Nothing is uploaded
- 会員登録・課金・広告がない / No account, no payment, no ads
- 閉じれば全部消える / Close the tab and everything is gone
- 1 ファイルで動く。ダブルクリックで開いても同じ / One file. Double-click it and it works the same

## できること（v1.0.0）/ What it does

| # | 効能 / Tool | 内容 / Details |
|---|---|---|
| 01 | 文字を書く / Text | タップ／クリックした場所にその場で入力。置いた文字はタップで書き直し、ドラッグで移動。日本語 OK。サイズ・色・複数行 / Type right where you tap or click. Tap placed text to edit, drag to move. Japanese OK. Size, colour, multi-line |
| 02 | 印影・画像 / Stamp, image | PNG（透過 OK）/ JPG を貼る。拡縮・移動 / Place PNG (transparency OK) or JPG. Resize, move |
| 03 | 手書き・署名 / Draw, sign | 指やマウスで描く。色・太さ / Draw with a finger or mouse. Colour, stroke width |
| 04 | 図形・マーカー / Shapes, highlight | 枠線・黄色マーカー・白塗り（修正液）・直線・矢印 / Box, yellow highlighter, white-out, line, arrow |
| 05 | 墨消し / Redact | 黒い箱を置くと、**そのページは画像化され下の文字は完全に消える** / Places a black box; **the page is rasterized and the text underneath is gone for good** |
| 06 | 結合・分割 / Merge, split | 複数 PDF を読み込んで並べ替え・削除、範囲指定で分割保存 / Load several PDFs, reorder, delete, save a page range |
| 07 | 回転 / Rotate | ページ単位・全ページ、90° ずつ / Per page or all pages, 90° steps |
| 08 | 白紙ページ / Blank page | A4・Letter・表示中のページと同サイズを差し込む / Insert A4, Letter or same-size blank pages |
| 09 | トリミング / Crop | ドラッグで範囲を決めて、このページ or 全ページに適用 / Drag a rectangle, apply to one page or all |
| 10 | 透かし / Watermark | 文字または画像を全ページ中央に。濃さ・角度 / Text or image on every page. Opacity, angle |
| 11 | ページ番号 / Page numbers | `{n} / {N}` などの書式、6 か所、開始番号、0 埋め（ベイツ番号）/ Formats like `{n} / {N}`, 6 positions, start number, zero padding (Bates) |
| 12 | フォーム記入 / Fill form | テキスト・チェック・ラジオ・ドロップダウン・リストに記入して確定（平坦化）/ Fill text, checkbox, radio, dropdown and list fields, then flatten |
| 13 | 情報 / Info | タイトル・作成者・サブタイトル・キーワード。読み込んだファイルの版・サイズ / Title, author, subject, keywords. Version and size of loaded files |
| 14 | 画像に変換 / To images | PDF → PNG / JPG（72・150・300 dpi、複数ページは zip）。PNG / JPG をドロップすれば画像 → PDF / PDF → PNG / JPG (72, 150, 300 dpi; zip for several pages). Drop PNG / JPG to go the other way |
| 15 | 圧縮 / Compress | 劣化なし（構造の最適化）と画像化（劣化あり・文字が検索不能になる旨を明記）/ Lossless (structure) and rasterize (lossy, text becomes unsearchable, and it says so) |
| 16 | パスワード / Password | AES-256 で保護（開く／権限、印刷・編集の禁止）。保護付き PDF はパスワードを聞いて外す / Protect with AES-256 (open / permissions, disallow print or edit). Protected PDFs ask for the password and come in unlocked |

**見る・動かす**: 全ページを縦に連続表示（Acrobat と同じ）。ページ番号を打って移動、← → / Home / End。最初は「選択・移動」モードで、紙をクリックしても何も置かれず、空いている所をドラッグすると紙が動きます（他の効能でも Space＋ドラッグ）。左右のパネルは上端の « » か `[` `]` で畳めます。
**View and move**: all pages in one continuous scroll (like Acrobat). Type a page number to jump, ← → / Home / End. The default mode is Select / pan: clicking the page places nothing, dragging empty space pans (Space + drag in any tool). Fold the side panels with the « » at their top or with `[` `]`.

**拡大・縮小**: ツールバーの ＋ / −、倍率の選択（幅に合わせる・全体を表示・25〜400%）、Ctrl＋ホイール（カーソルの下が動きません）、Ctrl＋＋ / Ctrl＋− / Ctrl＋0、スマホは2本指。
**Zoom**: + / − in the toolbar, a zoom menu (fit width, fit page, 25–400%), Ctrl+wheel (anchored under the cursor), Ctrl++ / Ctrl+- / Ctrl+0, or pinch on a phone.

**スマホ**: 上に効能、中央に紙、下に1行のバー。文字はその場で入力し、選んだ注釈の上に「書き直す・設定・削除」の小さなバーが出ます。設定はバーから出るシートで、設定から操作する効能を選んだときは自動で開きます。指で掴んで動かすと慣性で滑ります。2本指で拡大。
**Phone**: tools on top, the page in the middle, a one-line bar at the bottom. Text is typed in place, and a small bar (edit / settings / delete) appears above whatever you select. Settings slide up from the bar and open by themselves when you pick a tool that is operated from the panel. Drag with a finger to pan with momentum, pinch to zoom.

Ctrl+Z / Ctrl+Shift+Z、Ctrl+S、Ctrl+O、Delete、矢印キー、V / Esc（選択に戻る）、1〜9 のショートカットあり。
Shortcuts: Ctrl+Z / Ctrl+Shift+Z, Ctrl+S, Ctrl+O, Delete, arrow keys, V / Esc (back to select), 1–9.

## できないこと / What it cannot do

正直に書きます。以下は対応していません。**OCR 以外は対応する予定もありません。**
To be honest, these are not supported. **Apart from OCR, none of them are planned.**

| できないこと / Not supported | 理由・代わり / Why, and what to do instead |
|---|---|
| 既存の文字や画像そのものの書き換え / Editing existing text or images in place | 上から重ねることしかできません（白塗り＋文字入れで実質的に置き換えられます）/ You can only overlay (white-out + text does the job in practice) |
| Word・Excel・PowerPoint への変換 / Converting to Word, Excel, PowerPoint | ブラウザ内では品質が出ません / Cannot be done well inside a browser |
| PDF/A・PDF/X への変換 / PDF/A, PDF/X | 検証器なしに「準拠」と書けません / Cannot claim conformance without a validator |
| 証明書による電子署名 / Certificate-based digital signatures | 見た目の署名（手書き・画像）はできます。暗号署名は対象外 / A drawn or image signature is fine; cryptographic signing is out of scope |
| 2 つの PDF の比較 / Comparing two PDFs | — |
| OCR（文字認識）/ OCR | v1.2 で検討中。日本語の精度とダウンロード量が見合うかを先に試します / Under consideration for v1.2, pending accuracy and download size |
| XFA 形式のフォーム / XFA forms | AcroForm のみ / AcroForm only |

## 送らないもの / What never happens

PDF も画像も `FileReader` でブラウザのメモリに読むだけで、`fetch` / `XMLHttpRequest` でファイル本体を送る処理はコード上に存在しません。
ネットワークに出るのは、ライブラリ（pdf-lib / pdf.js / fontkit / qpdf-wasm）と日本語フォント、見た目用の Web フォントの取得だけです。
保存は Blob を `a[download]` で落とすだけ。`localStorage` に置くのは言語（`gp-lang`）と左右パネルの開閉（`gp-ui`）だけです。閉じれば全部消えます。

Your PDFs and images are read into browser memory with `FileReader`. There is no `fetch` / `XMLHttpRequest` in the code that sends a file anywhere.
The only network requests fetch libraries (pdf-lib / pdf.js / fontkit / qpdf-wasm), the Japanese font and the web fonts used for the UI.
Saving is a Blob handed to `a[download]`. The only things kept in `localStorage` are the language (`gp-lang`) and whether the side panels are folded (`gp-ui`). Close the tab and everything is gone.

確認方法 / How to check: ブラウザの開発者ツール → ネットワーク → ファイルを読み込んで操作 → POST が 1 件もないこと。
Open your browser's developer tools → Network → load and edit a file → there is not a single POST.

## 使い方 / How to use

1. https://ilove-ai.net/pdf を開く、または Releases の `index.html` をダウンロードしてダブルクリック
   Open https://ilove-ai.net/pdf, or download `index.html` from Releases and double-click it
2. PDF（または PNG / JPG）をドロップ / Drop a PDF (or PNG / JPG)
3. 左の効能を選んで操作 / Pick a tool on the left
4. 右上の「保存」/ Press Save in the top-right corner

ダウンロード版もライブラリとフォントはネットから取ります（オフラインでは動きません）。
The downloaded version still fetches libraries and fonts from the network (it does not work offline).

## 使っているもの / Built with

| ライブラリ / Library | ライセンス / License | 用途 / Used for |
|---|---|---|
| [pdf-lib](https://github.com/Hopding/pdf-lib) 1.17.1 | MIT | 書き出し / writing PDFs |
| [@pdf-lib/fontkit](https://github.com/Hopding/fontkit) 1.1.1 | MIT | フォント埋め込み / font embedding |
| [pdf.js](https://github.com/mozilla/pdf.js) 4.10.38 | Apache-2.0 | 表示・画像化 / rendering |
| [qpdf-wasm](https://github.com/jsscheller/qpdf-wasm) 0.0.2 | Apache-2.0 | パスワード・劣化なし圧縮（必要時だけ読み込み）/ passwords, lossless compression (loaded on demand) |
| [Noto Sans JP](https://github.com/notofonts/noto-cjk) | SIL OFL 1.1 | 日本語の文字入れ / Japanese text |

すべて CDN からバージョン固定で読み込みます。本体は **MIT License**（[LICENSE](LICENSE)）。
All pinned versions, loaded from CDNs. The app itself is **MIT** ([LICENSE](LICENSE)).

各社の商標は各社に帰属し、本ツールは各社と無関係です。
All trademarks belong to their respective owners. This tool is not affiliated with any of them.

## 開発 / Development

`index.html` がすべてです。ビルドも依存のインストールもありません。ブラウザで開いて直してください。
`index.html` is everything. No build step, no install. Open it in a browser and edit.

- 動作確認は headless Chromium で、16 効能の出力を pdf.js で読み戻して確かめています（座標・回転・暗号化・zip）
  Verified in headless Chromium by reading every tool's output back with pdf.js (coordinates, rotation, encryption, zip)
- バグ報告・要望は Issues へ / Bug reports and requests go to Issues
