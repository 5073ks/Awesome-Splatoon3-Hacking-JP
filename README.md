# Awesome-Splatoon3-Hacking
[DesperC](https://github.com/DesperC)によるスプラトゥーン3のハッキング/改造を学ぶためのリソースが入った非公式日本語版レポ

このレポは巨大なW.I.P.であり、非常に未完成です。このレポは[DesperC](https://github.com/DesperC)によるサイドプロジェクトです。

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

Flexlionはこれで完全にインストールされました！さあ、Modを入れてみよう

[Gamebananaのスプラトゥーン3 Mods](https://gamebanana.com/mods/games/15056)にアクセスして、Modを入手します。

これは単なる自己宣伝ではなく、[良いスタート用のMod](https://gamebanana.com/mods/439151)でもあります

`Comet Range Blaster`というタイトルのファイルをダウンロードし、`Source`と呼ばれるダウンロードは無視してください。Sourceには、Modを作成するために使用したソースファイルが含まれており、アップロードすることにしました。通常はMODと一緒に提出されるものではないが、誰かの役に立つかもしれないと思ったので

`Comet Range Blaster`フォルダー内の「romfs」フォルダーに移動します。次に、SDカード上のスプラトゥーン3のゲームIDフォルダーに移動し、7-Zipウィンドウから`romfs`フォルダーをSDカードの「romfs」フォルダーにドラッグします。

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/3ae70e5c-5905-411b-b252-b177e49fec57)

再度言いますが、これにより他のModがあっても自動的に置き換えが行われます。別のRange Blaster Modがインストールされている場合を除き、何かを上書きすることはありません。

SDカードを取り出し、Switchに入れて、再度atmosphere CFWを起動します。やり方を忘れた場合は、[このガイド](https://rentry.org/EristaEmuNAND#step-4)を参照してください。

良さそうだ！Modのインストール方法がわかったところで、次はModの作り方を見てみよう。基本的なUI画像置換Modの作り方を説明します

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

スクリーンショットのOSの不一致は無視してください。この一部は、管理者がWindows 11へのアップグレードを拒否している私の学校のノートパソコンで作成されました。

romfsのダンプがある場所に行ってください。`UI`フォルダーと`Icon`フォルダーを開いてください。以下はその概要です

![Screenshot 2023-05-10 125139](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/14ef08db-3caf-482f-bf14-b7f8dcd68ff4)

バッジとバナーのModを作ってみよう。まず、badgeフォルダから置き換えたいものを探します。

一見すると検索が不可能に見えるかもしれませんが、実際には非常に簡単です。すべてに慣れてくると、これらの名前を実際に読んで、中を開かずに何であるかを把握できるようになります。今のところは、すべてのファイルをPNGファイルとしてエクスポートして、どれを編集したいかを決めましょう

1. Switch Toolboxを開く
2. Tools > Batch Export Textures (All Supported Formats)に進みます
3. romfsディレクトリに移動し、ポップアップウィンドウから`UI/Icon/Badge`に戻ります
4. `Ctrl` + `A` ですべてのファイルを選択します
5. エンターキーを押します
6. 見つけやすいディレクトリに移動して、新しいフォルダーを作成してください。これは、プログラムに対して、以前に選択したすべてのテクスチャを選んだ見つけやすいディレクトリにエクスポートするよう指示するものです。私の場合は、すべての画像を保存するためにドキュメントフォルダー内に新しいフォルダーを作成しました。
7. エンターキーを押します
8. デフォルトで選択されていない場合は、Portable Graphics Networkを選択します
9. 上の3つのオプションのチェックを外すが、下の1つはチェックしたままにしておきます

<img width="182" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e755ec24-e3f1-4c76-980d-d7d5fd7174bd">

「OK」をクリックして、完了するまで待ちます。これは、すべてのテクスチャをエクスポートするために、進行状況バーのウィンドウを開いたり閉じたりしているだけなので、まるで痙攣しているかのように見えます。

エクスポートした場所に行ってください。ゲーム内のすべてのバッジアイコンが表示されるはずです。このチュートリアルでは、`Badge_Mission_Lv00`を選択します

10. お好みの画像編集ソフトウェアでバッジの画像を開きます。私はAdobe Photoshop 2024を使用しています。単に別の画像で「置き換える」ことができない理由は、その画像が正確に同じピクセルサイズでなければならないからです。
11. 好きな編集をしたり、そのスペースに好きな画像をはめ込んだり。画像の寸法を変えない限り、文字通り何でもできます。他のバッジの画像に置き換えることもできます。または、[このウェブサイト](https://seymourschlong.github.io/splashtags/)からカスタムバッジを入手することもできます。
12. 完成した画像をpngで保存します
13. romfsダンプのbadgeフォルダから、交換したバッジの名前を見つけてください

<img width="200" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/84ccb7e9-afe1-4290-be90-4874dcee39b1">

14. バッジファイルをSwitch Toolboxにドラッグ＆ドロップして開きます
15. アルバムアイコンの横にある`+`をクリックしてアルバムアイコンを開きます（横にプラスがない場合はダブルクリックしてください）。
16. 表示された画像をクリックします

<img width="662" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/6d590fdd-1d92-4c75-a38b-7d6c1d81c2ba">

17. ヒエラルキーの画像を右クリックし、`Replace`を選択します

<img width="218" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/b7772570-915d-49dd-bdc1-2a7582df1883">

18. カスタムバッジを保存した場所に移動し、選択します
19. 新しいオプションウィンドウで、フォーマットを `B8_G8_R8_A8_UNORM` に変更します。どのフォーマットが最も適しているかを見るために、すべてのフォーマットを交互に試すことをお勧めします。私の場合、このフォーマットはより柔らかいエッジとアルファチャンネル、そして良い色合いを提供します。フォーマットボックスを選択し、矢印キーを使って迅速に切り替えます。
20. OKをクリック
21. 右側の`Use SRGB`にカーソルを合わせ、ドロップダウンをクリックしてfalseからtrueに変更します

<img width="266" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/8340761b-601c-4b33-a6a6-ed687008599a">

22. 左上の保存アイコンをクリックします

<img width="215" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/74b2edd6-4fdd-4433-899b-0b4396c30e06">

23. 「ZSTDでファイルを圧縮しますか？」というウィンドウに 「はい 」をクリックします

これで、ツールボックスで開いたファイルが置き換えられました。romfsダンプのbadgeフォルダに戻り、先ほど置き換えたファイルを見つけてください

<img width="200" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/84ccb7e9-afe1-4290-be90-4874dcee39b1">

ヒント: ファイルの保存に成功したときにポップアップ表示される通知で、ファイルが保存された場所を確認できます
  
<img width="305" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/a711d13f-faad-4250-930a-5d1997bb52a2">

24. ファイルをコピーし、SDカードのゲームIDフォルダ（SD/atmosphere/contents）に移動します

25. romfsフォルダに入ります

26. `UI`というフォルダを作成します

27. そのフォルダの中に `Icon` というフォルダを作成します

28. そのフォルダの中に`Badge`というフォルダを作成します

29. そのファイルを `Badge` フォルダ内に貼り付けます

あなたはそのバッジを置き換えるためのModを作成しました！ご覧の通り、LayeredFSは与えられたファイルのみを置き換えるため、romfs内で置き換えたいファイルのディレクトリを再作成する必要があります。挑戦してみたい場合は、バナーを置き換えるモッドを作成してみてください。プロセスは同じですが、異なるフォルダと画像を使用します。バナーフォルダは `Npl` と呼ばれていることを忘れないでください。

# モデルのテクスチャの置き換え (旧)

この方法を残しておくことが誰かの役に立つかもしれませんが、現在は古くなっています。最新のチュートリアルについては、こちらをチェックしてください

面白いことを始める前に、もうひとつ無害な改造をしよう

1. Modelに入り、「Wmn」を検索してください。これですべての結果がフィルタリングされ、主要武器のモデルファイルだけが表示されます。

しかし、これらは画像ではないので、メイン、サブ、特殊な内部名称はすぐに覚えられるだろうが、どれがどれなのかを把握するために以前の方法を使うことはできません。とりあえず、どれがどれなのかのリストを以下に示します。また、これはファイル内で表示される順番でもあります。

### [このリストはSizzle Season 2023のものです](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#list-of-weapons-as-of-sizzle-season-2023)

2. お気に入りの武器を選択し、それをToolboxにドラッグします。
3. ファイルのドロップダウンとテクスチャのドロップダウンを開きます。

今は基本的な画像テクスチャAlbを修正しましょう。すべてのマップについて学びたい場合は、下にリストを作成しました。これらのテクスチャをいじることはお勧めしませんが、将来の参考のためにここに別のリストがあります。今は興味がない場合は、[リストの下](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#texture-names)にスキップしてください。

<img width="188" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/5d6ea7b9-787b-4434-b756-a1daef67d96a">

4. `Models`フォルダーを開き、モデルを .dae としてエクスポートします（複数のモデルがある場合は、すべてを .dae としてエクスポートしてください）

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c783d707-358c-485a-ad5c-c84c2c3224a6)

5. 覚えているディレクトリに移動します。そこにファイルを置くための新しいフォルダを作る。そのフォルダの中に保存してください。

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1e12ba1b-f9f1-4d7b-b2c6-cc567fa20e15)

### 6. 「Use Old Exporter」を有効にし、「Use Texture Channel Swaps」のチェックを外します

更新されたテクスチャチュートリアルから来たのであれば、25ステップまで進んでください。

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/8e74a838-d132-44a1-a4db-7b31d708d17a)

7. Blenderを開き、デフォルトのシーンオブジェクトを削除した後、.daeファイルをインポートします

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e7acea74-9225-4698-a9d9-38c95b595419)

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/b580dc9e-9320-4048-bdab-3469931ad9f8)

8. エディタのエッジを好みに合わせて調整します。その後、アウトライナーエディタをシェーダーエディタに変更します

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/0f00fe25-9aa0-4d0d-a331-c2d539c90690)

9. プリンシプルBSDFノードの`Specular`値を`0.5`に設定します

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/19224fec-741a-462c-b4c7-4b49e42b4e2d)

10. モデルに付属している各画像テクスチャ（`Alb`、`Mtl`、`Nrm`、`Rgh`）を、シェーダーエディターに1つずつドラッグ＆ドロップします。これらはプレビューを表示するための基本的なテクスチャです

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/7b6c3125-4b80-4cf7-a7ec-fd95d168ce8d)

11.`Shift` + `A`を使用して、テキストボックスに「nm」または「normal map」と入力し、ノーマルマップノードを作成します

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/7c872174-9f4d-484c-93bf-098992c714ab)

12. これはBlenderのチュートリアルではないので、ノードの設定が以下のようになることを確認してください。注目すべきは、囲まれているものとノードの接続だけです

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/a111b6b0-cac8-46c6-be8c-6186846811f0)

13. マテリアルプレビューモードをオンにします

 <img width="229" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/876af7dd-b6c2-43ed-a159-a167b54d5018">


14. あなたのモデルには複数のオブジェクトやマテリアルが含まれているかもしれません。その場合、正しく割り当てる方法は次のとおりです（複数のマテリアルがない場合は、ステップ15に進んでください）
  - モデルに複数のマテリアルがある場合、画像テクスチャファイルに1つ以上のプレフィックスが表示されます。このスクリーンショットには、合計3つのプレフィックスを持つ画像テクスチャファイルがあります。
  
  <img width="839" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1cbe5a0e-4bc6-498e-837c-91d94427e2b9">
  
  - For each prefix you have, there should also be a material. The material for each prefix should be on its respective object. To view all the objects, pull up the timeline window hiding at the bottom of the screen and change the clock icon to be the one labaled outliner.
  
  <img width="589" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c1c225e1-2f70-44bd-9304-be9c3fce29ee">
  
  - Press `Shift` + `A` to expand everything and locate everything reperesented by a triangle icon. those are your objects. Click on an object and go to the material properties
  
  <img width="950" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/2d8532dd-0bcd-434d-86ac-7c501f78e84b">
  
- Select the material and drag in the image textures which prefixes match the material name. Then repeat above process for each

<img width="482" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/fcf60101-03e0-40da-af58-6ac55123bc35">

- Your model could also have multiple models that actually use the same texture but it has a different material. If your image textures only have 1 prefix but some part of your model is still white, then assign the white model(s) the same material as the other model
 
15. Change the properties editor to a UV Editor
 
 <img width="616" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/2ff66f6b-992e-4608-9bda-75b2f4340201">

16. Open the image you want to edit. In this case, we are only editing the Alb image

 <img width="400" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/9b8d0372-5747-47cc-8caf-0badc5a61f48">

17. Back in the viewport, select the model, press `Tab` to switch to edit mode, and press `A` to select all vertecies. Your UV editor should be filled with orange dots and lines

 <img width="860" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/b504c7bc-eaee-4cf5-a28a-a565cd0a1fce">

18. In the UV editor, click the UV pannel and select Export UV Layout. You may need to scroll down the menu to see it.

 <img width="395" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/81a2f384-a201-4e3d-8fe2-8ca3d87b298d">

19. For organizational purposes, export the png file to the same place as all your image textures. Make sure to name it something that stands out

20. Open your photo editing program. Import the Alb texture and place the exported UV layout image on top of it. Now we can see how the model displays the texture.

21. Now go crazy. put anything you want on it. Remember not to change the size of the image though.

TIP: Remember to repeat the above process to get the UV layout for **ALL** of the objects that use the same material and put that UV map over the first one. You'll know if multiple objects are using the same material if there is some detail that looks like it should be covered by a UV layout.

22. Once done, hide the UV layout images so they dont appear in the final product. Export it in the same place as the original Alb image to replace it. we wont need it anymore

23. Back in the shader editor, click on the Alb node. then hit `N` to bring up a panel. Go to the `Node` section on that panel. Click the refresh button to refresh the image texture and make sure its to your liking

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/ca50a936-8e3d-460b-b504-b8a09a30255a)

25. Once ready, go back to toolbox and replace the Alb image on the model. The default settings in the window that pops up should be fine

<img width="229" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/dae238af-b5d9-4d09-b7dd-45052ed0588e">

**If you're following along with the new tutorial, return back to that section using [this link](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#9-save-the-bfres-file-using-the-save-icon-in-the-top-left-corner). if you're using this tutoairl because that method diddnt work, ignore this message.

26. Right click the `Textures` folder and click export

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e86377bc-3ea5-4f78-bb49-c98a1943e947)

27. Save it as `textures.bntx` to where your model and textures are

28. In toolbox, go to Tools > Compression > ZSTD > Decompress

29. Find your model in the models forlder and open it

30. Remove the `.zs.dec` in the name so the file extension becomes `.bfres`

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/79dd3b59-aeee-49c5-86a2-efd633ee198d)

31. Save it to where you originally exported the model

32. Open your hex editor. I'm using HxD

33. Drag the `.bfres` file into the hex editor to open it. You should now see a bunch of random characters

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/86474eaf-3767-4eb4-8435-107afaa873be)

34. Do the same for `textures.bntx` it should open in a new tab

35. Go to the `textures.bntx` tab and copy all of it (`Ctrl` + `A` then `Ctrl` + `C`)

36. Go back to the Wmn_Weapon_Name`.bfres` and hit `Ctrl` + `F`

37. Type in "bntx"

38. Click "Search All"

39. We want the line that has "BNTX" in all caps. That should always be the second line

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/f5a733bc-4c1d-4508-9bca-9ce4244b0ffe)

40. Click it to go to it.

41. Click Right before the highlighted portion (42 4E 54 58) right click and click "Paste Write." You should now see a lot of red text.

42. Hit `Ctrl` + `S` to save it. The text should be normal now. You can close the hex editor. (A `.bak` file might have been created. Ignore it)

43. Lets check if it worked. Drag the `.bfres` file into toolbox. If everything worked, you should see your textures on it now.

44. Go to Tools > Compression > ZSTD > Compress

45. Navigate to your folder with the `.bfres` file you just opened and select it.

46. Delete the "td" at the end of `zstd` on the file. it should now read Model_Name.bfres.zs

47. Now navigate to your `romfs` folder for your SD card where you keep mods for the game. Inside your `romfs` location, make a folder called "Model" if it isnt there already.

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/780d6b5e-5b70-4076-bce3-c84fd9d0f1b2)
ignore the 485348974563 mods I have in there its not important

49. Save the `.bfres.zs` inside the model folder

50. Boot up the game

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/95cf45d1-afa5-4a15-b22a-21152ccd8e6e)

Awesome! You just finished your own weapon reskin.


