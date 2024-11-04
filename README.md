# Awesome-Splatoon3-Hacking
[DesperC](https://github.com/DesperC)によるスプラトゥーン3のハッキング/改造を学ぶためのリソースが入った非公式日本語版Repo

このレポは巨大なW.I.P.であり、非常に未完成です。このRepoはDesperCによるサイドプロジェクトです。

もしあなたが行き詰まったり、助けが必要だと感じたら、[Splatoon Modding Hubディスコードサーバー](https://discord.com/invite/P6RNNvk)に気軽に参加してください。

この内容は殆ど古いので、まだ何か必要なら上のサーバーに参加して助けを求めてください。

オンラインでのMod/ハックの使用方法を教えるものではありませんし、オンラインでの使用は安全ではありません。後でバトルリプレイでのカメラハックの使用に関するセクションがあるかもしれませんが、それだけです。これらをオンラインで使用せずに、改造されたSwitchを正しくセットアップしてください。


# 目次
- はじめに
- 必要なもの／必須要件
- テクスチャの置き換え（旧）
  - テクスチャの置き換え
  - モデルの置き換え
  - テキストの置き換え
  - オーディオの置き換え
- RomFSのダンプ
  - エミュレーターの使用
  - Switchの使用
- セーブデータのエクスポート・編集・インポート
- Modの使い方/インストール方法
- ファイル形式（参考用）
- 最初のMod（チュートリアル）

# はじめに
このセクションには元々、改造されたSwitchとエミュレーターのセットアップに関するリンクが含まれていましたが、どちらも海賊行為のため削除されました。ただし、どちらも見つけるのは難しくありません。

# 必要なもの／必須要件
これらは、ハッキングの旅をサポートするために必要なものです。これらはすべてゲーム改造のためのものであり、Switchのハッキングやカスタムファームウェア（CFW）の設定のためのものではありません。CFWの設定に関するガイドは、上記のセクションを参照してください。

- [Flexlion Mod Menu](https://flexlion.github.io/)
- [スプラトゥーン3 Save Editor (from flexlion)](https://flexlion.github.io/saveeditor.html)
- [Switch Toolbox](https://github.com/KillzXGaming/Switch-Toolbox)
- [7-Zip](https://www.7-zip.org/) zipファイルをデフォルトで開くように、7-Zipをメインのアーカイブアプリとして設定することを強くお勧めします
- [完全なスプラトゥーン3セーブデータ](https://ptb.discord.com/channels/410208534861447168/830855276437438485/1081218616734793738) （あなたのセーブデータがすでに必要なものすべてを持っていて、かつEdiZonを使用してセーブデータをファイルとしてエクスポートする方法を知っている場合は、これをスキップできます）。ファイルにアクセスできない場合は、たとえRyujinxを使用していなくても、[Ryujinxのディスコードサーバー](https://discord.gg/ryujinx)に参加して入手する必要があります。これはエミュレーターとSwitchの両方で動作します

以下は、ゲームの特定の側面を置き換えるために必要なプログラムに関するサブセクションです。***これは、改造可能な全てのもののリストではありません。あくまで、特定の改造に必要な他のプログラムのリストです。***

### テクスチャの置き換え（旧）
- Hex Editor. どんなHex Editorでもいい。個人的には [HxD](https://mh-nexus.de/en/)
- Image Editor (Duh)
- [Blender](https://www.blender.org/) テクスチャがモデル上でどのように見えるかを確認

### テクスチャの置き換え
- Image Editor (still, duh)
- [Blender](https://www.blender.org/) テクスチャがモデル上でどのように見えるかを確認

### モデルの置き換え
- [Blender](https://www.blender.org/) または他の3Dエディターとその使い方の知識が必要。基本的に3Dモデルの経験が必要

### テキストの置き換え
- [Kuriimu](https://github.com/IcySon55/Kuriimu) または [Kuriimu 2](https://github.com/FanTranslatorsInternational/Kuriimu2)
Kuriimu 2はより永続的なインストール方式であり、Kuriimuは軽量でポータブルなソリューション

### オーディオの置き換え
- [Looping Audio Converter](https://github.com/libertyernie/LoopingAudioConverter)
- [Citric Composer](https://gota7.github.io/Citric-Composer/)
- [Automatic BARS Patcher](https://github.com/ic-scm/automatic-bars-patcher) or [Online BARS Patcher](https://smashcustommusic.net/onlinetools/bars-patcher/)
- [Foobar2000](https://www.foobar2000.org/) + [VGMStream](https://www.foobar2000.org/components/view/foo_input_vgmstream)
- オーディオエディター。 個人的には [Audacity](https://www.audacityteam.org)

# RomFSのダンプ

### エミュレータ (初心者推奨) (Switchを使用しない場合は必須)
（インストールしたいアップデートやDLCがある場合は、NSP形式でインストールしてください）ゲームを右クリックし、「RomFSをダンプ」を選択します。**これらのファイルをどこにダンプしたかを必ず覚えておくか、覚えやすい場所に置いておいてください。**

### Switch（初心者向けではない）
Lockpick_RCMとNxdumptoolが必要

Lockpick_RCMへのリンクは許可されていませんが、Githubの多くの場所で見つけることができます

その後、この[動画](https://www.youtube.com/watch?v=mKw2ips97og)を見て使い方を学びます

それが終わったら、[Nxdumptoolのnroファイル](https://github.com/DarkMatterCore/nxdumptool/releases)をダウンロードします

次に、この[動画](https://www.youtube.com/watch?v=BZpK2JT8lcI)を見てそれの使い方を学びます

私が自分で説明しない理由は、このガイドがゲームの改造に焦点を当てているためで、セットアップについては説明していないからです

# セーブデータのエクスポート・編集・インポート
まずはセーブファイルを取得する必要があります。自分のセーブファイルを改造することもできますし、[必須ダウンロード](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#essentials)にあるものをダウンロードすることもできます

自分のセーブファイルを使用する場合は、[EdiZonのnroファイルをダウンロード](https://github.com/WerWolv/EdiZon/releases/tag/v3.1.0)してください

ダウンロードが完了したら、[このチュートリアル](https://www.cfwaifu.com/edizon-saves/)を参照して、完全なセットアップの方法を確認してください

次に、[スプラトゥーン3 Save Editor](https://flexlion.github.io/saveeditor.html)にアクセスして、セーブデータの殆どすべてを変更し、その後、再ダウンロードしてください（新しいセーブファイルの名前が変更されている場合は、再び `save.dat` に戻す必要があります）

スプラトゥーン3に再インポートするには、上記のチュートリアルの後半を参照してください

# Modの使い方/インストール方法
最初のMODを作成する前に、実際にインストールする方法を学ぶ必要があります。SDカードのルートを開いてください（エミュレーターの場合は仮想SDカードのルートへ）

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/4b9f7abb-1085-4121-bbbb-ade78938816b)

atmosphereフォルダを開いて、`contents`という名前のフォルダを作成します。このフォルダは、私たちのModを保存する場所になります。atmosphereには、ゲーム起動時にゲームファイルを置き換えるための組み込みツールであるLayeredFSがあります。

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/67c2034b-5030-4bc9-bdc7-7827703a3056)

まず、contentsフォルダの中に`0100C2500FC20000`という名前のフォルダを作成します。これはスプラトゥーン3のゲームIDです。他のゲームのModがある場合は、それらのゲームIDを使ってさらにフォルダを作成します。

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1e734bc1-00da-46b2-b9c0-45f03f49804b)

ゲームIDフォルダを開き、`romfs`というフォルダを作成します。しかし、MODをインストールするときは、MODファイルに関連するディレクトリだけを再作成します。多くの場合、この作業はすでに終わっています。とりあえず、Flexlionと、テクスチャか何かを置き換える他のMODをセットアップしてましょう。SDカードのルートに戻ってFlexlionのrarファイルを開き、7-ZipからSDカードのルートに両方のフォルダをドラックします。これですべてのファイルが必要な場所に自動的に配置されます。

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/fa9e5974-2c8f-4f7b-a81e-55c6e1ed08a7)

Flexlionはこれで完全にインストールされました！さあ、MODを取り付けよう

[Gamebananaのスプラトゥーン3 Mods](https://gamebanana.com/mods/games/15056)にアクセスして、Modを入手します。

これは単なる自己宣伝ではなく、[良いスタート用のMod](https://gamebanana.com/mods/439151)でもあります

`Comet Range Blaster`というタイトルのファイルをダウンロードし、`Source`と呼ばれるダウンロードは無視してください。Sourceには、Modを作成するために使用したソースファイルが含まれており、アップロードすることにしました。通常はMODと一緒に提出されるものではないが、誰かの役に立つかもしれないと思ったので

`Comet Range Blaster`フォルダー内の「romfs」フォルダーに移動します。次に、SDカード上のスプラトゥーン3のゲームIDフォルダーに移動し、7-Zipウィンドウから`romfs`フォルダーをSDカードの「romfs」フォルダーにドラッグします。

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/3ae70e5c-5905-411b-b252-b177e49fec57)

再度言いますが、これにより他のModがあっても自動的に置き換えが行われます。別のRange Blaster Modがインストールされている場合を除き、何かを上書きすることはありません。

SDカードを取り出し、Switchに入れて、再度atmosphere CFWを起動します。やり方を忘れた場合は、[このガイド](https://rentry.org/EristaEmuNAND#step-4)を参照してください。

良さそうだ！MODのインストール方法がわかったところで、次はMODの作り方を見てみよう。基本的なUI画像置換MODの作り方を説明します

# ファイル形式（参考用）
なぜスプラトゥーン3はromfsフォルダ内で`.zs`ファイルしか使わないのか不思議に思うかもしれません。ZS は実は ZSTD Compression の略で、ファイルの末尾に `.zs` をつけるだけです。以下は、ファイルの中にあるその他のファイル形式です。いくつかのファイルは、私がそれらについての知識を持っていないため、まだここに文書化されていません。

- `.zs` ゲームファイル全体でZSTD圧縮を使用

- `.bfres` モデル・テクスチャ・アニメーション・マテリアルなどを含む3Dモデルファイル。今のところ、暗号化されているため、テクスチャ以外のすべてを置き換えることはできません

- `.pack` 文字通り、他の多くのファイルを含むパッケージです。私たちが扱うのは実際には1つの`.pack`ファイルだけですが、それが殆どすべてを制御しています。しかし、それについては後に説明します。通常、ゲームのパラメータが含まれています

- `.sarc` ほとんどの`.sarc`ファイルは、/Malsにある言語ファイルです。通常、メッセージバイナリテキストファイル（`.msbt`）が含まれています
  - `.msbt` には、ゲームが各言語ファイルのために使用するテキストが含まれています。Toolboxで開くことはできますが、編集して保存するにはKuriimuのような別のプログラムが必要

- `.bfarc` Fontにあるフォントファイルを含むファイル（通常のフォントと同様にリッピングしてインストールすることが可能）

- `.bgyml`, `.gyml`, `.byml`, YAMLファイルの種類。通常はプロパティを定義

- `.bntx` 画像を含む。多くは/UI/Iconにあります

- `.blarc` UI要素を表示する方法をゲームに指示するレイアウトファイル（テクスチャ用の`.bntx`ファイルを含む）
  - `.bflyt` UI画像を画面上にどのように配置・アニメーションするかをゲームに指示するレイアウトの一部
  - `.bflan` レイアウトファイルのアニメーションファイル

- `.bars` ゲームオーディオを含むファイル。Switch Toolboxでは使用できないが、他のプログラムで編集可能
  - `.bwav` バイナリWAVファイル。通常は.barsファイルの中にあるが、/Sound/Resource/Streamにもあります


# 最初のMod（チュートリアル）
