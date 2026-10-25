# PinSharp ICO

[![Latest Release](https://badgen.net/github/release/chililikobo/PinSharpICO)](https://github.com/chililikobo/PinSharpICO/releases/latest)
[![Downloads](https://badgen.net/github/assets-dl/chililikobo/PinSharpICO)](https://github.com/chililikobo/PinSharpICO/releases/latest)
[![License](https://badgen.net/badge/license/Free/purple)](#editions--licensing)
[![Platform](https://badgen.net/badge/platform/Windows%2011/black)](https://chililikobo.github.io/en/PinSharpICO.html)

[English](#english) | [日本語](#日本語)

---

## English

PinSharp ICO is a high-definition Windows icon (`.ico`) generator designed to produce sharp, highly legible icons from 256×256 PNG images. It eliminates common issues found in standard downscaling tools—such as muddy gray outlines, lost dark slits, and white halo artifacts—ensuring fine lines and vibrant details stay crystal clear even at tiny display sizes like 16×16 and 24×24.

### Key Features

* **Automated Processing on Drag-and-Drop**: Simply drag and drop your 256×256 PNG image into the window (or click to browse). The conversion begins immediately, and the generated `.ico` file is automatically saved into the same folder as the source PNG with zero extra clicks.
* **Full Coverage of All 11 Standard Windows Sizes**: Supports 16, 20, 24, 32, 40, 48, 64, 72, 96, 128, and 256 px. Easily toggle target sizes using convenient presets (All, Standard, Compact) or individual buttons.
* **Ultra-Sharp Downscaling for Tiny Sizes**: Dedicated perceptual downscaling engine preserves contrast for thin outlines, dark slits, and accent colors at 16×16 and 24×24 without jagged pixelation.
* **Halo-Free Robust Clamping**: Mathematical local bounding box clamping completely eliminates unwanted white fringing and ringing artifacts around edges.
* **Direction-Adaptive Upscaling**: Built-in edge-directed interpolator smoothly scales smaller input images while suppressing stair-step jaggedness along diagonal and curved edges.
* **Small-Size Preview Thumbnails**: Displays up to 5 result preview thumbnails in ascending order (smallest first) right after generation for instant legibility verification.
* **Native AOT Compiled**: Built with .NET 10 (Native AOT) as a standalone portable application with no external .NET runtime requirements.

### Quick Start

1. Extract the downloaded ZIP archive and place the entire folder in any directory.
*(Keep the required DLLs like `Magick.Native-Q8-x64.dll`, `libSkiaSharp.dll`, `libHarfBuzzSharp.dll`, and `av_libglesv2.dll` in the same folder as `PinSharpICO.exe`.)*
2. Launch `PinSharpICO.exe`.
3. Select your target sizes if necessary (All 11 sizes are enabled by default).
4. Drag and drop your **256×256 PNG** file into the window (or click the drop zone to browse).
5. The `.ico` file is automatically saved into the source folder as `[SourceFileName].ico` (or `[SourceFileName] (1).ico` if an identical file exists) alongside instant preview thumbnails.

### License

* **Free Edition**: Free to use for both personal and commercial purposes.

### Terms & Disclaimer

* **Redistribution**: Secondary distribution is strictly prohibited in principle. Please link to the official website or repository.
* **Data Privacy**: No external transmission of image files or personal data.
* **Warranty**: Provided "As-Is". The author assumes no responsibility whatsoever for any damages resulting from the use of this software.

### Third-Party Licenses (Credits)
This application incorporates open-source components. For detailed copyright notices and license agreements, refer to [ThirdPartyNotices.md](ThirdPartyNotices.md).

### Links & Contact

* **Developer**: chilili kobo
* **Website**: [https://chililikobo.github.io/en/](https://chililikobo.github.io/en/)
* **X (Twitter)**: [@chililikobo](https://x.com/chililikobo)
* **Email**: chilili.kobo@gmail.com

---

## 日本語

PinSharp ICO（ピンシャープ・アイコ）は、256×256ピクセルのPNG画像から、極小サイズでも線や文字がぼやけず、くっきりと見やすいWindows用アイコンファイル（`.ico`）を生成する専用ユーティリティです。一般的な縮小ツールで起きがちな「16×16での白線のグレー沈み」「黒い隙間の消失」「輪郭の白フチ浮き（ハロー現象）」を防ぎ、全解像度でシャープなアイコンを出力します。

### 主な機能

* **ファイルを落とすだけの「全自動保存」**: 256×256のPNG画像をドラッグ＆ドロップする（または画面をクリックして選択する）だけで即座に変換が始まり、元のPNGと同じフォルダへICOファイルを自動保存します（保存ダイアログや保存ボタンを押す手間はありません）。
* **Windows標準の全11サイズ（16〜256px）対応**: 16, 20, 24, 32, 40, 48, 64, 72, 96, 128, 256 px の全サイズを網羅。All (11)、Standard (6)、Compact (4) のプリセットボタンや個別ボタンで必要なサイズを自由に選択できます。
* **極小サイズ特化の高鮮明縮小**: 16×16や24×24の極小解像度でも、細い枠線や黒いスリット、アクセントカラーの彩度が背景に埋もれず、パキッと浮かび上がります。
* **ハロー（白フチ浮き）ゼロの境界クランプ**: セル内ロバスト極値クランプにより、アンシャープマスク等で発生する不自然な輪郭の白浮きを原理的に排除しています。
* **方向適応型アップスケール**: 入力画像が小さい場合でも、斜め線や円弧の階段状ジャギーを抑えて滑らかに拡大補間します。
* **小さい順に最大5つの仕上がりプレビュー**: 処理完了後、視認性を確認したい小さいサイズ順に最大5つのプレビューが表示されます。
* **Native AOT コンパイル**: .NET 10 (Native AOT) により単体で軽快に動作し、.NETランタイムなどの追加インストールは不要です。

### 使い方

1. ダウンロードしたZIPアーカイブを展開し、フォルダごと任意の場所に配置します。
*(動作に必要な `Magick.Native-Q8-x64.dll`、`libSkiaSharp.dll`、`libHarfBuzzSharp.dll`、`av_libglesv2.dll` は `PinSharpICO.exe` と同じフォルダに置いたままにしてください。)*
2. `PinSharpICO.exe` を起動します。
3. 必要に応じて画面下部のボタンで含めたいサイズを選択します（標準では全11サイズが選択されています）。
4. **256×256ピクセルのPNG画像**を画面中央へドラッグ＆ドロップします（画面をクリックしてファイル選択も可能）。
5. 変換が完了すると、元のPNGと同じフォルダに `[元のファイル名].ico`（既存の場合は `[元のファイル名] (1).ico`）として自動保存され、プレビューが表示されます。

### ライセンス

* **Free Edition**: 個人利用・商用利用を問わず、完全無料でご利用いただけます。

### 利用規約・免責事項

* **再配布**: 二次配布は原則として禁止します。公式サイトや本リポジトリへのリンクを推奨します。
* **外部通信**: 画像データや個人情報をインターネット上へ無断送信することは一切ありません。
* **免責事項**: 本ソフトウェアは「現状有姿（As-Is）」で提供され、使用により生じた一切の損害について作者は責任を負いません。

### サードパーティ・ライセンス（クレジット）
本ソフトウェアはオープンソースコンポーネントを使用しています。各コンポーネントの著作権表示およびライセンス条文の詳細は [ThirdPartyNotices.md](ThirdPartyNotices.md) をご参照ください。

### リンク・連絡先

* **制作者**: chilili kobo
* **ウェブサイト**: [https://chililikobo.github.io/](https://chililikobo.github.io/)
* **X (旧Twitter)**: [@chililikobo](https://x.com/chililikobo)
* **メール**: chilili.kobo@gmail.com
