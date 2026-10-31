# PinSharp ICO

[![Latest Release](https://badgen.net/github/release/chililikobo/PinSharpICO)](https://github.com/chililikobo/PinSharpICO/releases/latest)
[![Downloads](https://badgen.net/github/assets-dl/chililikobo/PinSharpICO)](https://github.com/chililikobo/PinSharpICO/releases/latest)
[![License](https://badgen.net/badge/license/Free%20%2F%20Pro/purple)](#pro-edition--licensing)
[![Platform](https://badgen.net/badge/platform/Windows/black)](https://chililikobo.github.io/en/pinsharpico.html)

[English](#english) | [日本語](#日本語)

---

## English

PinSharp ICO is a fast and easy-to-use Windows icon (`.ico`) generator designed to produce crisp, highly legible icons from images. It eliminates common downscaling issues—such as muddy gray outlines, clogged dark slits, and blurred shapes—ensuring fine lines, typography, and details stay sharp even at tiny sizes like 16×16 and 24×24.

Simply drag and drop an image into the window, and your icon is ready in an instant!

### Edition Comparison (Free vs Pro)

| Feature | Free Edition | Pro Edition |
| :--- | :--- | :--- |
| **Windows Standard Sizes (11 sizes)** | Yes (16px to 256px) | Yes (16px to 256px) |
| **Ultra-Sharp Small-Size Scaling** | Yes | Yes |
| **Multi-Size 1:1 Result Previews** | Yes (Up to 5 smallest sizes) | Yes (Up to 5 smallest sizes) |
| **Bilingual UI (EN / JA Toggle)** | Yes ([F2] key) | Yes ([F2] key) |
| **Settings Persistence** | Yes (`settings.json`) | Yes (`settings.json`) |
| **Supported Image Formats** | **PNG only** (`.png`) | **PNG, JPEG, BMP, WebP** |
| **Batch & Folder Conversion** | 1 file at a time | **Multi-file & recursive folders** |
| **Shape Masks (Icon Clipping)** | Square (Unclipped) | **Square, Rounded, Circle** |
| **Output Destination Routing** | Same folder as source | **Same folder, `icons/` subfolder, Custom folder** |
| **Command Line Interface (CLI)** | Not supported | **Fully supported** (headless automation) |
| **License Model** | Free (Personal & Commercial) | One-time purchase (Lifetime license) |

### Key Features

* **Automated Save on Drag-and-Drop**: Simply drag and drop an image into the window (or click to browse). The conversion starts immediately, and the generated `.ico` file is automatically saved without needing to click any "Save" buttons.
* **Full Coverage of All 11 Standard Windows Sizes**: Supports 16, 20, 24, 32, 40, 48, 64, 72, 96, 128, and 256 px. Switch between convenient presets (All, Standard, Compact) with one click.
* **Ultra-Sharp Downscaling for Tiny Sizes**: Fine borders, text, and tight slits stay crisp and high-contrast instead of blurring into the background.
* **Multi-Size Result Previews**: Displays up to 5 preview thumbnails in ascending order (smallest first) right after generation for instant legibility verification.
* **Multiple Image Formats Supported [Pro]**: Directly converts PNG (`.png`), JPEG (`.jpg` / `.jpeg`), BMP (`.bmp`), and WebP (`.webp`).
* **Batch Multi-File & Recursive Folder Conversion [Pro]**: Drop multiple images to convert them in sequence, or drop an entire folder to automatically discover and convert all supported images inside subfolders.
* **Modern Shape Masks [Pro]**:
  * **Square**: Standard unclipped icon.
  * **Rounded**: Sleek, modern rounded corners like popular desktop & mobile apps.
  * **Circle**: Round circular icon ideal for avatars and badges.
  *(Non-square images are automatically centered and cleanly clipped).*
* **Flexible Output Destinations [Pro]**: Save alongside the original image, automatically create an `icons/` subfolder, or choose any custom folder. Existing files are safely numbered `(1), (2)...` to avoid accidental overwrites.
* **Command Line Interface (CLI) Automation [Pro]**: Run batch conversions directly from Command Prompt, PowerShell, or local build scripts without opening the GUI. *(Note: Cloud-hosted ephemeral CI/CD environments such as GitHub Actions runners are not supported due to machine-bound license activation.)*
* **Multi-Language GUI & Persistent Settings**: Press `[F2]` or click the language badge to toggle between English and Japanese. All options are automatically remembered for future launches.
* **Native AOT Compiled**: Built with .NET 10 (Native AOT) as a standalone portable application. No .NET runtime installation required.

### Quick Start (GUI)

1. Extract the downloaded ZIP archive and place the folder anywhere.
   *(Keep the bundled DLLs in the same folder as `PinSharpICO.exe`.)*
2. Launch `PinSharpICO.exe`.
3. Pick your preferred sizes, shape [Pro], and output destination [Pro] (optional).
4. Drag and drop your image file (or folder [Pro]) into the center area.
5. The `.ico` file is automatically generated and saved! Click **Show in Explorer** to open the output folder.

### Command Line Usage (CLI) [Pro Edition]

PinSharp ICO can be executed directly from the terminal or scripts:

```bash
# Simplest conversion (saves .ico next to source image)
PinSharpICO.exe "app_icon.png"

# Convert image with modern rounded corners
PinSharpICO.exe "photo.jpg" --shape rounded

# Convert image with circular mask
PinSharpICO.exe "avatar.webp" --shape circle

# Batch-convert an entire folder with rounded corners to an output directory
PinSharpICO.exe "D:\Assets\Images" -o "D:\Assets\Icons" --shape rounded

# Automatically save into an 'icons/' subfolder
PinSharpICO.exe "D:\Assets\Images" --subfolder

# Generate only specific sizes
PinSharpICO.exe "icon.png" -s 16,32,48,256
```

### Pro Edition & Licensing

* **How to Buy**: Click the **Upgrade to Pro** button in the upper-right corner of the window, or visit our store on Gumroad:
  * **Store URL**: [https://chililikobo.gumroad.com/l/vefjk](https://chililikobo.gumroad.com/l/vefjk)
  * **Pricing**: One-time purchase (Lifetime license, no subscriptions).
* **Activation**:
  1. Click **Upgrade to Pro** in the app header.
  2. Enter your License Key and purchase Email address received from Gumroad.
  3. Click **Activate** to instantly unlock all Pro features.
* **Device Usage & Portability**:
  * The license is for the purchaser's own use on their PCs (it can be reactivated when switching to a new PC).
  * If you encounter any issues reactivating after replacing or upgrading your PC, please feel free to contact support at [chilili.kobo@gmail.com](mailto:chilili.kobo@gmail.com).
  * Internet access is only needed once during initial activation; after that, it works completely offline.
  * To uninstall, simply delete the folder.

### Terms & Disclaimer

* **Licensing**:
  * **Free Edition**: Free to use for both personal and commercial purposes.
  * **Pro Edition**: Licensed for use by the purchaser on their own PCs. Sharing, transferring, or reselling license keys is strictly prohibited.
* **Redistribution**: Secondary distribution is strictly prohibited in principle. Please link to the official website or repository.
* **Privacy & Network**: No image files or personal data are ever uploaded to any server. Network access is only used during Pro license verification.
* **Warranty**: Provided "As-Is". The author assumes no responsibility whatsoever for any damages resulting from the use of this software.

### Third-Party Licenses

For detailed copyright notices and license agreements, refer to [ThirdPartyNotices.md](ThirdPartyNotices.md).

### Links & Contact

* **Developer**: chilili kobo
* **Website**: [https://chililikobo.github.io/en/](https://chililikobo.github.io/en/)
* **X (Twitter)**: [@chililikobo](https://x.com/chililikobo)
* **Email**: [chilili.kobo@gmail.com](mailto:chilili.kobo@gmail.com)

---

## 日本語

PinSharp ICO（ピンシャープ・アイコ）は、画像からWindows用のアイコンファイル（`.ico`）を誰でもかんたんに作成できる高画質アイコン生成ツールです。

一般的なツールで起きがちな「小さいサイズでの線のぼやけ」「文字や隙間の黒つぶれ」「輪郭のにじみ」を解消し、16×16や24×24などの極小サイズでもくっきりパキッとした見やすいアイコンを自動で作成します。

画像を画面に「ポイッ」とドラッグ＆ドロップするだけで、面倒な設定なしですぐにきれいなアイコンが完成します。

### エディション比較（Free版とPro版）

| 機能項目 | Free Edition | Pro Edition |
| :--- | :--- | :--- |
| **Windows標準全11サイズ対応** | ○（16px〜256px） | ○（16px〜256px） |
| **極小サイズ高鮮明処理** | ○ | ○ |
| **仕上がりプレビュー表示** | ○（小さい順に最大5サイズ） | ○（小さい順に最大5サイズ） |
| **日英UI言語切り替え** | ○（[F2] キー） | ○（[F2] キー） |
| **設定の自動保存** | ○（`settings.json`） | ○（`settings.json`） |
| **対応画像フォーマット** | **PNG のみ**（`.png`） | **PNG, JPEG, BMP, WebP** |
| **一括変換（バッチ処理）** | 1ファイルずつ | **複数ファイル ＆ フォルダ一括（再帰探索対応）** |
| **形状マスク（アイコン切り抜き）** | 四角形（クリップなし） | **四角形、角丸、円形** |
| **スマート出力先フォルダー管理** | 元画像と同じフォルダー | **同じフォルダー、`icons/` サブ、任意指定パス** |
| **コマンドライン実行 (CLI)** | 非対応 | **完全対応**（スクリプト自動化） |
| **料金・ライセンス** | 無料（個人・商用問わず） | 有料買い切り（永久ライセンス） |

### 主な機能

* **画像を落とすだけの「全自動保存」**: 画像をウィンドウにドラッグ＆ドロップするだけで処理がスタートし、完了と同時に自動保存されます（保存ボタンを押す手間はありません）。
* **Windows標準の全11サイズ（16〜256px）対応**: 16, 20, 24, 32, 40, 48, 64, 72, 96, 128, 256 px を網羅。All / Standard / Compact のプリセットボタンでワンクリック切り替えが可能です。
* **小さいサイズでも潰れない高鮮明処理**: 16×16や24×24などの極小サイズでも、細い枠線や文字、隙間のコントラストをしっかり保ち、くっきり浮かび上がらせます。
* **小さい順に5つの仕上がりプレビュー**: 変換後、特に確認したい小さいサイズ順にプレビューが表示され、仕上がりをすぐにチェックできます。
* **いろいろな画像形式に対応【Pro限定】**: PNG画像に加えて、写真やイラストでよく使われるJPEG（`.jpg` / `.jpeg`）、BMP（`.bmp`）、WebP（`.webp`）の読み込みに対応しています。
* **複数ファイル＆フォルダごと一括変換【Pro限定】**: 複数の画像をまとめてドラッグ＆ドロップして一括変換できます。フォルダをドロップすれば、サブフォルダ内も含めて対応画像を自動探索してまとめてアイコン化します。
* **角丸や丸型のアイコンに切り抜き【Pro限定】**:
  * **四角形（Square）**: 元の形のまま出力。
  * **角丸（Rounded）**: モダンなアプリアイコン風のおしゃれな角丸。
  * **円形（Circle）**: アバターやバッジに最適なまあるい丸型アイコン。
  *(正方形でない画像も、自動で中央に合わせて綺麗に切り抜きます)*
* **便利な保存先設定【Pro限定】**: 「元画像と同じ場所」「iconsフォルダを自動作成して保存」「好きなフォルダを指定して保存」から選べます。同名ファイルがある場合は自動で `(1), (2)...` と連番が付くため安全です。
* **コマンドライン（CLI）自動化【Pro限定】**: コマンドプロンプト、PowerShell、ローカルのビルドスクリプト等から直接アイコン作成を実行できます（※PC固有のライセンス認証を行っているため、使い捨てのクラウドCI/CD環境［GitHub-hostedランナー等］には対応しておりません）。
* **日本語・英語の切り替え ＆ 設定の自動保存**: 右上の言語ボタン、またはキーボードの `[F2]` キーでいつでも日本語と英語を切り替えられます。選んだサイズや設定は次回起動時にも自動で引き継がれます。
* **Native AOT コンパイル**: .NET 10 (Native AOT) により単体で軽快に動作し、.NETランタイムなどの追加インストールは不要です。

### 使い方（GUI）

1. ダウンロードしたZIPアーカイブを展開し、フォルダごと任意の場所に配置します。
   *(同梱のDLLファイルは `PinSharpICO.exe` と同じフォルダに置いたままにしてください。)*
2. `PinSharpICO.exe` をダブルクリックして起動します。
3. 必要に応じてサイズ・形状【Pro】・保存先【Pro】を選択します（標準で全サイズが選択されています）。
4. 画像ファイル（またはフォルダ【Pro】）を画面中央へドラッグ＆ドロップします。
5. 一瞬でアイコンファイル（`.ico`）が生成・保存されます。「エクスプローラーで表示」ボタンで出力先をすぐに確認できます。

### コマンドラインからの使い方（CLI）【Pro版限定】

コマンドプロンプトやPowerShellから直接実行できます。

```bash
# 1. 画像をアイコンにする（一番シンプル）
PinSharpICO.exe "my_icon.png"

# 2. 写真をおしゃれな角丸アイコンにする
PinSharpICO.exe "photo.jpg" --shape rounded

# 3. イラストを丸型アイコンにする
PinSharpICO.exe "avatar.webp" --shape circle

# 4. フォルダ内の全画像を角丸にして別のフォルダへ一括保存
PinSharpICO.exe "D:\Images" -o "D:\Icons" --shape rounded

# 5. 画像と同じ階層の 'icons/' フォルダに自動保存
PinSharpICO.exe "D:\Images" --subfolder

# 6. 生成するサイズを限定して高速変換
PinSharpICO.exe "icon.png" -s 16,32,48,256
```

### Pro版の購入とライセンス登録

* **購入方法**: 画面右上の「Pro へアップグレード」ボタンをクリックするか、以下の販売ページ（Gumroad）からご購入いただけます。
  * **購入ページ**: [https://chililikobo.gumroad.com/l/vefjk](https://chililikobo.gumroad.com/l/vefjk)
  * **価格体系**: 買い切り（月額料金などは一切かかりません）。
* **ライセンス登録手順**:
  1. 画面右上の「Pro へアップグレード」ボタンをクリックします。
  2. 購入後にメールで届いた「ライセンスキー」と「メールアドレス」を入力します。
  3. 「有効化」ボタンを押すと、即座にすべてのPro機能が使えるようになります。
* **ライセンスの仕様と安心設計**:
  * ご購入いただいたご本人が管理するパソコンでご利用いただけます（PCの買い替え時も再認証可能です）。
  * 万が一、PCの買い替え等で再認証ができない場合は、お手数ですがサポート（[chilili.kobo@gmail.com](mailto:chilili.kobo@gmail.com)）までお気軽にお問い合わせください。
  * 初回の登録時だけインターネット通信を行いますが、一度登録すれば普段はオフライン（ネット接続なし）でも問題なく動きます。
  * アンインストール時はフォルダごとゴミ箱へ捨てるだけで完全に消去できます。

### 利用規約・免責事項

* **ライセンスについて**:
  * **Free版**: 個人利用・商用利用を問わず、どなたでも無料で自由に使えます。
  * **Pro版**: ご購入いただいたご本人が管理するPCで利用できます。ライセンスキーを他人に教えたり、転売・共有することはできません。
* **二次配布**: 二次配布は原則として禁止します。公式サイトや本リポジトリへのリンクをお願いいたします。
* **プライバシー・外部通信**: お手持ちの画像データや個人情報をインターネット上に送信することは一切ありません。Pro版のライセンス登録時のみ、正規購入を確認するための通信を行います。
* **免責事項**: 本ソフトウェアは「現状有姿（As-Is）」で提供され、使用により生じた損害について作者は一切の責任を負いません。

### サードパーティ・ライセンス

オープンソース・ライブラリのライセンス表示については、[ThirdPartyNotices.md](ThirdPartyNotices.md) をご確認ください。

### リンク・連絡先

* **制作者**: chilili kobo
* **ウェブサイト**: [https://chililikobo.github.io/](https://chililikobo.github.io/)
* **X (旧Twitter)**: [@chililikobo](https://x.com/chililikobo)
* **メール**: [chilili.kobo@gmail.com](mailto:chilili.kobo@gmail.com)
