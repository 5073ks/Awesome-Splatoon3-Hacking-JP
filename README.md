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

8. エディタのエッジを好みに合わせて調整します。その後、Outliner EditorをShader Editorに変更します

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/0f00fe25-9aa0-4d0d-a331-c2d539c90690)

9. プリンシプルBSDFノードの`Specular`値を`0.5`に設定します

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/19224fec-741a-462c-b4c7-4b49e42b4e2d)

10. モデルに付属している各画像テクスチャ（`Alb`、`Mtl`、`Nrm`、`Rgh`）を、Shader Editorに1つずつドラッグ＆ドロップします。これらはプレビューを表示するための基本的なテクスチャです

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
  
  - 各プレフィックスごとに、それぞれのマテリアルが必要です。各プレフィックスのマテリアルは、それぞれのオブジェクトに配置されているべきです。すべてのオブジェクトを表示するには、画面の下に隠れているタイムラインウィンドウを表示し、時計のアイコンを「アウトライナー」と表示されているものに変更します。
  
  <img width="589" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c1c225e1-2f70-44bd-9304-be9c3fce29ee">
  
  - `Shift` + `A`を押してすべてを展開し、三角形のアイコンで表されているすべてのものを見つけます。それらがあなたのオブジェクトです。オブジェクトをクリックし、マテリアルプロパティに移動します
  
  <img width="950" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/2d8532dd-0bcd-434d-86ac-7c501f78e84b">
  
- マテリアルを選択し、対応するプレフィックスを持つイメージテクスチャをドラッグします。次に、上記のプロセスを各マテリアルについて繰り返します

<img width="482" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/fcf60101-03e0-40da-af58-6ac55123bc35">

- あなたのモデルには、実際に同じテクスチャを使用する複数のモデルがある場合もありますが、それぞれ異なるマテリアルを持っています。イメージテクスチャにプレフィックスが1つしかない場合でも、モデルの一部がまだ白いままであるなら、その白いモデルに他のモデルと同じマテリアルを割り当ててください
 
15. プロパティエディターをUVエディターに変更します
 
 <img width="616" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/2ff66f6b-992e-4608-9bda-75b2f4340201">

16. 編集したい画像を開きます。この場合、私たちはAlb画像のみを編集しています

 <img width="400" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/9b8d0372-5747-47cc-8caf-0badc5a61f48">

17. ビューポートに戻り、モデルを選択して`Tab`を押して編集モードに切り替え、`A`を押してすべての頂点を選択します。あなたのUVエディターにはオレンジの点と線が満たされているはずです

 <img width="860" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/b504c7bc-eaee-4cf5-a28a-a565cd0a1fce">

18. UVエディターで、UVパネルをクリックし、「UVレイアウトをエクスポート」を選択します。メニューをスクロールしないと見えないかもしれません。

 <img width="395" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/81a2f384-a201-4e3d-8fe2-8ca3d87b298d">

19. 整理のため、pngファイルをすべての画像テクスチャと同じ場所にエクスポートします。必ず目立つ名前をつけてください。

20. 写真編集ソフトを開きます。Albテクスチャをインポートし、エクスポートしたUVレイアウト画像をその上に配置します。これで、モデルがテクスチャをどのように表示するかを見ることができます。

21. 好きなものを好きなように貼ってください。ただし、画像のサイズは変えないように。

ヒント: 他のオブジェクトが同じマテリアルを使用している場合、UVレイアウトを取得するために上記のプロセスを繰り返すことを忘れないでください。すべてのUVマップを最初のものの上に配置します。同じマテリアルを使用しているかどうかは、UVレイアウトでカバーされるべき詳細があるかどうかを確認することでわかります。

22. 完成したら、UVレイアウト画像を非表示にして、最終製品に表示されないようにします。元のAlb画像と同じ場所にエクスポートして置き換えます

23. Shader Editorに戻り、Albノードをクリックします。その後、`N`を押してパネルを表示させます。パネルの`Node`セクションに移動し、Refreshボタンをクリックして画像テクスチャを更新し、満足のいく状態になっていることを確認します

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/ca50a936-8e3d-460b-b504-b8a09a30255a)

25. 準備ができたら、ツールボックスに戻り、モデル上のAlb画像を置き換えます。ポップアップするウィンドウのデフォルト設定でOK

<img width="229" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/dae238af-b5d9-4d09-b7dd-45052ed0588e">

**新しいチュートリアルに沿っている場合は、[このリンク](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#9-save-the-bfres-file-using-the-save-icon-in-the-top-left-corner)を使用してそのセクションに戻ってください。この方法が上手くいかなかった為にこのチュートリアルを使用している場合は、このメッセージを無視してください。**

26. `Textures`フォルダを右クリックし、エクスポートをクリックします

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e86377bc-3ea5-4f78-bb49-c98a1943e947)

27. モデルとテクスチャがある場所に`textures.bntx`として保存します

29. Toolboxで、Tools > Compression > ZSTD > Decompressを選択します

30. モデルフォルダーでモデルを見つけ、それを開きます

31. ファイル名の`.zs.dec`を削除し、拡張子が`.bfres`になるようにします

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/79dd3b59-aeee-49c5-86a2-efd633ee198d)

31. モデルを最初にエクスポートした場所に保存します

32. Hex Editorを開きます。私はHxDを使用しています

33. `.bfres`ファイルをHex Editorにドラッグして開きます。これでランダムな文字がたくさん表示されるはずです

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/86474eaf-3767-4eb4-8435-107afaa873be)

34. 同じように`textures.bntx`を新しいタブで開きます

35. `textures.bntx`タブに移動し、すべてをコピーします（`Ctrl` + `A` 次に `Ctrl` + `C`）

36. Wmn_Weapon_Name`.bfres` に戻り、`Ctrl` + `F` キーを押します

37. 「bntx」と入力します

38. 「Search All」をクリックします

39. 「BNTX」と大文字で書かれている行を探します。それは常に2行目にあるはずです

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/f5a733bc-4c1d-4508-9bca-9ce4244b0ffe)

40. クリックするとそのページに移動します。

41. ハイライトされた部分（42 4E 54 58）の直前を右クリックし、「Paste Write」をクリックします。すると、多くの赤いテキストが表示されるはずです。

42. `Ctrl` + `S`を押して保存します。テキストが正常になっているはずです。これで、Hex Editorを閉じても大丈夫です（`.bak`ファイルが作成されているかもしれませんが、無視して構いません）

43. 上手くいったか確認しましょう。.bfres`ファイルをツールボックスにドラッグしてください。上手くいけば、テクスチャが表示されるはずです。

44. Tools > Compression > ZSTD > Compressにを選択します

45. 先ほど開いた`.bfres`ファイルがあるフォルダに移動して、そのファイルを選択します

46. ファイル名の末尾にある「td」を削除します。これでファイル名は「Model_Name.bfres.zs」となります

47. 次に、ゲームのために mods を保存している SD カードの `romfs` フォルダーに移動します。まだ存在しない場合は、その中に「Model」というフォルダーを作成します。

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/780d6b5e-5b70-4076-bce3-c84fd9d0f1b2)
そこにある 485348974563 の mod は無視してください。重要ではありません

49. `.bfres.zs`をモデルフォルダ内に保存します

50. ゲームを起動してください

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/95cf45d1-afa5-4a15-b22a-21152ccd8e6e)

素晴らしい！あなたは自分の武器のリスキンを完成させたよ！

# テクスチャの置き換え

**この方法はまだ実験段階です。失敗した場合は、テクスチャの置き換えガイドを参照してください。この方法の方が信頼性が高いですが、少し時間がかかります。**

お気に入りの武器のベーステクスチャを変更するMODを作りましょう

1. まず、`romfs/Model`フォルダーに入って、`Wmn`を検索します。これにより、主な武器モデルのみが表示されるように結果がフィルタリングされます。

もしギアのパーツを変更したい場合、私の友人のJohn#1878がDiscordで作成した、3.0.0までのすべてのギアのコーディネート名と画像のリストがあります

[アタマ](https://docs.google.com/document/d/1SaQOljCMUCjGNYzhnbqUHCXR1vrdef67vUVbcv_2Lkg/edit)

[フク](https://docs.google.com/document/d/1bIje-QhxGa0EThWjB5V9xj_Jqfj9D8Bjkb-Wu9ruNSg/edit)

[クツ](https://docs.google.com/document/d/1MwfrztugDbqNlU6S87Oflz-WQrSwxC20zV25aqNwn9k/edit)

### Sizzle Season 2023の武器リスト

`Blaster_Coop` Grizzco Blaster

`Blaster_Light` Rapid Blaster + Rapid Blaster Pro

`Blaster_Light_Cstm01` Rapid Blaster Deco

`Blaster_Light_Cstm11` Rapid Blaster Pro Deco

`Blaster_LightShort` Clash Blaster

`Blaster_LightShort_Cstm01` Clash Blaster Neo

`Blaster_Long` Range Blaster

`Blaster_Middle` Blaster

`Blaster_Precision` S-Blast 92

`Blaster_Short` Luna Blaster

`Blaster_Short_Cstm01` Luna Blaster Neo

`Brush_Heavy` Painbrush

`Brush_Mini` Inkbrush

`Brush_Mini_Cstm01` Inkbrush Nouveau

`Brush_Normal` Octobrush

`Charger_Coop` Grizzco Charger

`Charger_Keeper` Goo Tuber

`Changer_Light` Bamboozler 14 Mk I (my beloved)

`Charger_Long` E-Liter + E-Liter Scoped

`Charger_LongB` Splatoon 2 E-Liter (For Amiibo)

`Charger_NormalT` Splat Charger

`Charger_NormalT_Cstm01` Zekkofin Charger

`Charger_Pencil` Snipewriter 5H

`Charger_Quick` Squiffer

`Maneuver_Dual` Dualie Squelchers

`Maneuver_Dual_Cstm01` Custom Dualie Squelchers

`Maneuver_Gallon` Glooga Dualies

`Maneuver_NormalT` Splat Dualies

`Maneuver_Short` Dapple Dualies

`Maneuver_Short_Cstm01` Dapple Dualies Nouveau

`Maneuver_Stepper` Dark Tetra Dualies

`Maneuver_Stepper_Cstm01` Light Tetra Dualies

`Roller_BrushNormal` Splatoon 2 Octobrush (For Amiibo)

`Roller_Compact` Carbon Roller

`Roller_Compact_Cstm01` Carbon Roller Deco

`Roller_Heavy` Dynamo Roller

`Roller_Heavy_Cstm01` Gold Dynamo Roller (Not Released)

`Roller_Hunter` Flingza Roller

`Roller_NormalT` Splat Roller

`Roller_NormalT_Cstm01` Krak-On Splat Roller

`Roller_Wide` Big Swig Roller

`Roller_Wide_Cstm01` Big Swig Roller Express

`Saber_Coop` Grizzco Splatana

`Saber_Light` Splatana Wiper (Wiper can also be seen in other places named `Saber_Lite` instead)

`Saber_Light_Cstm01` Splatana Wiper Deco

`Saber_Normal` Splatana Stamper

`Shelter_Compact` Undercover Brella

`Shelter_Coop` Grizzco Brella

`Shelter_Normal` Splat Brella

`Shelter_Wide` Tenta Brella

`Shelter_Wide_Cstm01` Sorella Tenta Brella

`Shooter_Blaze` Aerospray MG

`Shooter_Blaze_Cstm01` Aerospray RG

`Shooter_Expert` Splattershot Pro

`Shooter_Expert_Cstm01` Forge Splattershot Pro

`Shooter_First` Splattershot Jr.

`Shooter_FirstCstm01` Custom Splattershot Jr.

`Shooter_Flash` Squeezer

`Shooter_Gravity` .52 Gal

`Shooter_Heavy` .96 Gal

`Shooter_Heavy_Cstm01` .96 Gal Deco

`Shooter_Long` Jet Squelcher

`Shooter_Long_Cstm01` Custom Jet Squelcher

`Shooter_Msn0Lv0` Hero Shot (All 3 Phases)

`Shooter_Normal` Splatoon 1 Splattershot (For Amiibo)

`Shooter_NormalB` Splatoon 2 Splattershot (For Amiibo)

`Shooter_NormalT` Splattershot

`Shooter_NormalT_Cstm01` Tentatek Splattershot

`Shooter_QuickLong` Splattershot Nova

`Shooter_QuickLong_Cstm01` Anakai Splattershot Nova

`Shooter_Quickmiddle` N-Zap 85

`Shooter_QuickMiddle_Cstm01` N-Zap 89

`Shooter_RvLv0` Rival Octolong Octoshot (Hero Mode)

`Shooter_Short` Sploosh-o-Matic + Splash-o-Matic

`Shooter_Short_Cstm01` Sploosh-o-Matic Neo

`Shooter_Short_Cstm11` Splash-o-Matic Neo

`Shooter_Triple` L-3 Nozzlenose

`Shooter_Triple_Cstm01` L-3 Nozzlenose D

`Shooter_TripleMiddle` H-3 Nozzlenose

`Shooter_TripleMiddle_Cstm01` H-3 Nozzlenose D

`Slosher_Bathtub` Bloblobber

`Slosher_Coop` Grizzco Slosher

`Slosher_Diffusion` Tri-Slosher

`Slosher_Diffusion_Cstm01` Tri-Slosher Nouveau

`Slosher_Launcher`Sloshing Machine

`Slosher_StrongT` Slosher

`Slosher_StrongT_Cstm` Slosher Deco

`Slosher_Washtub` Explosher

`Spinner_Downpour` Ballpoint Splatling

`Spinner_HyperT` Hydra Splatling

`Spinner_QuickT` Mini Splatling

`Spinner_QuickT_Cstm01` Zink Mini Splatling

`Spinner_Serein` Nautilus 47

`Spinner_StandardT` Heavy Splatling

`Spinner_StandardT_Cstm01` Heavy Splatling Deco

`Stringer_Coop` Grizzco Stringer

`Stringer_Normal` Tri-Stringer

`Stringer_Short` REEFLUX-450

これをタイプするのに45分かかったと言ったら信じてくれますか？

今は、ベース画像テクスチャAlbを変更しましょう。すべてのマップについて学びたいなら、下にリストを作りました。まだこれらのテクスチャをいじることはお勧めしませんので、これは将来の参考用の別のリストです。興味がなければ、そのリストの下にスキップしてください。

### テクスチャの名前
`Alb - Albedo` ベース画像テクスチャ。`Diffuse`、`Diff`、または`Dif`とも呼ばれることがある

`Mlt` ベース画像テクスチャ **Mtl テクスチャと混同しないでください**

`Tcl - Team Color` 特定のモデルの部分をチームのインクの色とその強さを示す画像マスク。黒は強度0、灰色は明るさに応じて0から1の範囲、白は強度1を意味する

`Ao - Ambient Occlusion` 基本テクスチャにディテールや影を追加します。**Nrmテクスチャの目的や機能と混同しないでください。**

`Mtl - Metalness` 特定の部分を金属的にするための画像マスクであり、その強さを示します。黒は0の強度、灰色は0から1の強度（暗いまたは明るいほど）、白は1の強度を意味する

`Rgh - Roughness` 特定の部分に指定された粗さの値を持たせるための画像マスクです。黒は0の強度、灰色は0から1の強度（暗いまたは明るいほど）、白は1の強度を意味する

`Nrm - Normal Map` 画像から抽出したベクターを使用して、モデルの表面に非常に細かいディテールを追加します。モデルのジオメトリを追加することなく、見た目もとても美しい

`2cl - Ink Damage Effect` これは、ダメージを受けたときにモデルのどこに敵のインク素材を表示するかをゲームに指示するために使用されます。黒は0の強度を意味し、灰色は明るさに応じて0から1の間の強度を持ち、白は1の強度を意味する

`Mfk - Secondary Normal Map` モデルと組み合わせて見ることが非常に珍しいマップです。これはモデルにさらに細かいディテールを加える役割を果たしますが、扱うのが非常に面倒

`Opa - Opacity` モデルの特定の部分に不透明度の値を設定するために使用されます。黒は0の強度、灰色は0から1の強度（明るさや暗さに応じて）、白は1の強度を意味する

`Emm - Emission` モデルのどの部分が光を発する必要があり、その強さをどのように設定するかを示す画像マスクです。黒は0の強度、灰色は0から1の強度（明るさや暗さに応じて）、白は1の強度を意味する

`Trm - Transmission` モデルにサブサーフェススキャッタリング効果をエミュレートするために使用されます。基本的には、これらに手を出さない方が良い

`Thc - Thickness` 伝送をより良く見せるのに役立ちます。常に Trm テクスチャとペアになっています。黒は 0 強度、灰色は暗さや明るさに応じて 0 から 1 の強度、白は 1 強度を意味する

`Hlt / Mac - Highlight` 何かを非常に光沢のあるものにするために使用されます。黒は 0 強度、灰色は暗さや明るさに応じて 0 から 1 の強度、白は 1 強度を意味する

`Rft - Lightwarp` [フレネル効果](https://www.3drender.com/glossary/fresneleffect.htm#:~:text=Fresnel%20Effect%20(pronounced%20"fre-,depends%20on%20the%20viewing%20angle.))をエミュレートし、色も表現する

`Fxm - Effect Mask` さまざまな材質特有の効果をマスクするために使用されます。黒は0の強度を意味し、灰色は明るさに応じて0から1の強度を示し、白は1の強度を意味する

`Hlm - Lightwarp Effect Mask` ライトワープテクスチャをマスクするために使用されます。黒は0の強度を意味し、灰色は明るさに応じて0から1の強度を示し、白は1の強度を意味する

`Mlta / Mltb - Special Effects` 何にでも使用できます。特に決まった用途はなし

`Mai - Skin Mask` モデルのどの部分が肌であり、どの部分が肌でないかを定義するために通常使用される画像マスクです。黒は0の強度、灰色は明るさに応じて0から1の強度（暗いまたは明るい）を意味し、白は1の強度を意味する

出典: [PastaOwOのSquidnodesマテリアルとテクスチャのWiki](https://github.com/PastaOwO/Squidnodes/wiki/Materials-and-Textures?scrlybrkr=c562aa65)

2. ファイルを解凍するには、Tools > Compression > ZSTD > Decompress に移動し、見つけやすい場所に保存してください。
3. 解凍した `.bfres` ファイルをToolboxにドラッグします。
4. モデルフォルダをクリックします。
5. 修正したいテクスチャ(s)を使用しているモデルを右クリックします。
6. `.bfres`と同じフォルダに`.dae`としてエクスポートします。
7. `Use Old Exporter`にチェックを入れ、`Use Texture Channel Swaps`のチェックを外します。
8. もう一度説明するのが面倒なので、古い方法の[このセクション](https://github.com/DesperC/Awesome-Splatoon3-Hacking/blob/main/README.md#6-toggle-use-old-exporter-and-untoggle-use-texture-channel-swaps)を参照してください。

### 9. Save the .bfres file using the save icon in the top left corner

10. Recompress the file using Tools > Compression > ZSTD > Compress and compress the bfres file
11. remove the "td" at the end of `zstd` to make it just say 'zs' and then save that file to the model folder of your sd card romfs directory.

TIP : You can combine these 2 modding tecniques that you've learned so far to create custom icons and badges for your reskin just like my [Comet Range Blaster mod!](https://gamebanana.com/mods/439151) To learn how to make 2D icons from 3D models, here is a link to a small tutorial inside the repo. (TO BE MADE)

# Replacing Text.
This is how i made my Google Translate Mod. Hours of copying text from the game and putting it through translate a million times. Cant believe im gonna do the same thing for side order

Anyways enough of my crippling anxiety, lets start by [downloading the required editor](https://github.com/DesperC/Awesome-Splatoon3-Hacking?scrlybrkr=c562aa65#text-replacement)

I would reccomend setting Kuriimu as your default .msbt editing program so you dont need to drag the file in the program to open it every time.

1. In your romfs dump, open the Mals folder. i'm assuming youre language is english so we want this file right here

<img width="224" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1d31f2c2-80d4-4efc-9c39-24d676f2721e">

2. Drag the file into toolbox to open it. there are a ton of .msbt files in here so here is a small list of where important ones are as well as important prefixes

any files starting with `msn` or `mission` or any files located inside the `LogicMsg` folder or any files in `CommonMsg/Mission` relate to hero mode

any files starting with `vs` or `versus` or `lobby` relate to multiplayer

you can find the splashtag titles files in `CommonMsg/Byname`

weapon names are in `CommonMsg/Weapon` 

try looking at the glossary file in `CommonMsg/Glossary.msbt` if you want to find names of characters

gear names can be found at `CommonMsg/Gear`

text relating to salmon run is any file that has `Coop` or `LobbyCoop` in the name

if you want to edit what Deep Cut says on the news, search for any files starting with `News`

Toolbox cant edit the msbt files so we need to export them to edit them.

3. Find any `.msbt` files you want. right click on them and click Export Raw Data

<img width="305" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/abb00fc6-c6d7-4173-8fc5-d071411ac62a">

4. Save the file to a place you will remember

5. open Kuriimu then open the .msbt file with Kuriimu by dragging it over

6. click yes to keep a backup. this is very helpful for multiple reasons then just if you need to revert

<img width="295" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/9724c759-6e35-438c-acbb-95893a3eb744">

7. Click this icon here to get a preview inside the text entries

<img width="249" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e6a1cb3c-c657-4cbf-8087-5ecf5f25cfdb">

Dont worry if the entry names are gibberish. We never need to worry about names

remember you can always use these 2 options to find something(s) specific (first one) or find and replace something(s) specific (second one)

<img width="128" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/cf9ac1e0-ef99-4658-8414-9b0b806417db">

8. Once you edit everything you want to edit, do `Ctrl` + `S` to save the file.

9. back in toolbox, right click the file you just exported but now click Replace Raw Data

<img width="349" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/0258b0d8-5105-4fec-bafb-3c6ff27b77dd">

10. Navigate to the `.msbt` file you edited with Kuriimu. You should also see a `.bak` file there. ignore it

11. select the `.msbt` file

12. back in toolbox, double click the file you just replaced to open a preview of it to make sure it has your edits. toolbox can preview msbt files but it cant edit them.

<img width="454" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/11143db9-66b6-47fa-88d8-70a99814a37a">

13. Close the pop up window and save the file 

<img width="142" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c4973c0c-a84e-4e64-ae3f-60f862ef4ff8">

14. Click Yes to the promt

<img width="148" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/f12a659b-2218-4a5a-a392-6499eedb39e9">

15. Copy the `.sarc` file we just edited and navigate to your SD card romfs directory. Make a new folder called Mals and paste the file in there

16. Boot up the game

NOTE: You will need to 

Text editing is one of the simplest but most effective ways of modding in my opinion. I really enjoy making characters just say the dumbest things.

# Editing UI Layouts

Not started yet but you can use when ive already taught you to edit the files in the Layout folder

# Replacing Audio
This is completely optional. If you wanna learn how to actually get into the _hacking_ part of this then skip to the next section. Otherwise follow this tutorial

cant be bothered to write out my own right now. might do this last. for now, refer to [this tutorial](https://gamebanana.com/tuts/15422)

# Custom Kits
Time for your first game hack. Weapon kits are stored in romfs/RSDB/`WeaponInfoMain.Product.GAME_VERSION.rstbl.byml.zs`

Before we get started, here is a list of all the subs and specials that can go on weapons

`SpBlower` Ink Vac

`SpCastle` Kraken

`SpChariot` Crab Tank

`SpEnergyStand` Tacticooler

`SpFirework` Super Chump

`SpGachihoko` Rainmaker

`SpGreatBarrier` Big Bubbler

`SpInkStorm` InkStorm

`SpJetpack` Inkjet

`SpMicroLaser` Killer Wail 5.1

`SpMultiMissile` Tenta Missiles

`SpNiceBall` Booyah Bomb

`SpShockSonar` Wavebreaker

`SpSkewer` Reefslider

`SpSuperHook` Zipcaster

`SpSuperLanding` Splashdown (yes really)

`SpTripleTornado` Tristrike

`SpUltraShot` Trizooka

`SpUltraStamp` Ultra Stamp

Sub Weapons, if there are parenthesis next to a name, that tells you its second name that can be seen in the files on occasion. The second names arent too important i just put them there so you would know.

`Beacon` Beacon (`Flag`)

`Bomb_Curling` Curling Bomb

`Bomb_Fizzy` Fizzy Bomb (`Bomb_Piyo`)

`Bomb_Quick` Burst Bomb (`Bomb_Handy`)

`Bomb_Robot` Autobomb (`Bomb_Robo`)

`Bomb_Splash` Splat Bomb

`Bomb_Suction` Suction Bomb (`Bomb_Hold`)

`Bomb_Torpedo` Torpedo (`Bomb_Tako`)

`LineMarker` Line Marker (`LinMarker`)

`PointSensor` Point Sensor (`MarkingBall`)

`PoisonMist` Toxic Mist (`DevillBall`)

`SalmonBuddy` Lil' Buddy - Needs to be modified if you want to use it on a weapon

`Shield` Splash Wall

`Sprinkler` Take a guess

`Trap` Ink Mine

Alright. Now we can get to editing kits.

1. Open switch toolbox and go to Tools > Compression > ZSTD > Decompress

2. Go to your romfs dump and go inside RSDB. Select `WeaponInfoMain.Product.GAME_VERSION.rstbl.byml.zs`

3. Delete the ".zs.dec" at the end of the file name so you're left with ".bfres" as the extension

4. save the file in a place so it will be easy to find.

5. go to where you saved the file and drag it into toolbox

6. Use [this list](https://github.com/DesperC/Awesome-Splatoon3-Hacking/edit/main/README.md#this-list-is-as-of-fresh-season-2023) again to find your weapon.

7. switch to text editor and hit "Decompile." hit `Ctr` + `F` and type in the weapon codename. dont use any underscores

8. Find the paragraph that looks like this relating to your weapon

<img width="667" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/23a2d883-8a23-4a45-b500-83361f70bc08">

9. The only notable things you can change in this file are:

- Weapon kits

- Weapon Special Points

- What badges you get from getting 4 and 5 star on that weapon

- Weapon UI Values (a.e the game showing you how much range the weapon has)

- Weapon ID. This is a bit more complicated and is explained what it is and how to do later in the guide.

10. Right now, we will only need to look at these 3 lines

<img width="518" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/1dce16e1-0f11-4276-9370-b8a132ec3ec4">

Note that this isnt the correct kit for Bamboozler because i have already messed with it. Dosent change the process for changing any weapon kit though

11. Lets replace the special first. Copy the special codename you want from the list above and replace the original special

This is the only part of the line that needs to be fully replaced with your special

<img width="494" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e9e302e7-83bb-4650-9501-d1d57da15a3b">

12. Now do the same thing for the sub weapon. Again this is the only part that should be replaced 

<img width="437" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/c8ec91e7-a01a-433f-9461-73ec9a66bcc6">

13. If you feel like it, edit the required amount of special points for the weapon. Setting it to 0 will automatically fill the special meter again after you use it

<img width="143" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/09f8ba82-3738-48f9-aac7-37de715b1366">

Dont worry about the `!l` thats just telling the game that its a Int32 value meaning it can store values up to 2,147,483,647

14. compile it by clicking "Compile" near the top of the window

<img width="297" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/49ec7fbd-24d3-4399-aa9f-9b4e2fa0e226">

15. Now save it with the save icon

<img width="250" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/d1290a51-21b4-438e-b469-b1eec8d5774e">

Finally, we need to recompress it

16. go to Tools > Compression > ZSTD > Compress

17. select the .byml you just saved

18. delete the "td" at the end of the file name so the end of the file reads `.rstbl.byml.zs`

19. navigate to the romfs folder on your sd card. Make a folder called RSDB and place the file in there

20. Boot up the game

Have fun with your new kit but be sure to take a little break if all that code overwhelmed you because the next tutorial will involve a lot of code as well.

# Changing Weapon Functionality / Parameters

This might be the most anticipated part for you. At the end of this walkthough you will be able to change almost anything about any main, sub, and special weapon.

Right now i will just show you how to modify some very basic parameters. After this tutorial though is where everything gets more specific and i show you literally everything i know

Lets change the range, damage, RNG, and fire rate of the Splattershot Nova

This tutorial will have less pictures and less descriptive text for things we've already done multiple times in previous tutotials.

1. Inside toolbox, lets decompress another file with ZSTD compression. You should know how to decompress and compress with ZSTD by now

2. go to your romfs dump and open the Pack folder. Then select `Params.pack.zs`

This file contains all main, sub, special weapon parameters as well as stage parameters

3.  save it as `Params.pack` to a location you can find easily

4.  open the newly saved `Params.pack` in toolbox

We are going to search for the code name of a weapon we want to modify. If you want to modify its functionality specifically for salmon run or hero mode, add `_Msn` for hero mode or `_Coop` for salmon run to the end of the search.

5.  Hit the search button and search for ShooterQuickLong. To find splattershot nova. however this brings up 2 files

<img width="107" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/6b72cce2-f1b0-4ee2-bf7b-95f0b0ef3a21">

<img width="304" alt="image" src="https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/e33eb047-ff30-4360-8afc-baad4aae8a06">

We always want the one that dosent have "Coop" in the name. Coop means Co-op which means salmon run. any file in Params.pack with Coop in the name only changes specific parts of the weapon in salmon run so we dont care about it.

6. Click the file without Coop in the name to locate it in the file view. Close the search window now

7. double click the highlighted file.

8. switch to text editor and hit "Decompile"

Lets start by giving it 100 damage just for the hell of it.

9. Locate the line that says DamageParam. Should be at line 15

10. ValueMax and ValueMin are the only values we care about 

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/3f69a8f3-b325-4806-b846-fc88b141207f)

11. 240 and 120 are the damage numbers multiplied by 10. the extra zero is in case a decimal value is needed. so lets set the Max and Min damage to 1000 to make it do 100 damage no matter what.

12. Lets also give nova perfect RNG. To do this, scroll down to the bottom section `WeaponParam`

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/4fd0b12c-24ee-442a-924e-0151b75ae3b9)

13. RNG is under the 2 variables that contain `DegSwerve` Jump_DegSwerve is jump RNG and Stand_DegSwerve is ground RNG. set them both to 0

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/3a20c4bc-2cec-49c0-aa3b-9442c2587d87)

14. now on to fire rate. the `RepeatFrame` variable. Set it to 1 to make it fire every frame. i dont know what setting it to 0 will do and im too scared to try

15. Finally, range. scroll up to the line called `MoveParam` (should be line 18) and find the variable called `SpawnSpeed`. this is the range. but because its so small, just adding 1 or 2 will make it shoot across the map. although you can set this as high or as low as you want. Set the highlighted value on this line to a larger number
![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/fa70d5a0-4ef8-4cae-8843-8a4df3d4853f)

16. click Compile at the top

17. once you save that file, make sure to save the Params.pack file too

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/b00f54ea-b1f0-455c-a2c0-421ab5982f02)

18. compress the saved file with ZSTD. and put your newly created `Params.pack.zs` inside the Pack folder in your SD card romfs directory

![image](https://github.com/DesperC/Awesome-Splatoon3-Hacking/assets/121410727/d0844ef8-1f92-4672-b676-60ac8be23e4b)

29. Boot up the game

Nova is finally a functioning weapon. 

# Specific Weapon Parameters
This section will have sub sections that all focus on telling you where and how to modify more specific weapon functionality. general functions of a class will not be covered as they are either unimportant or easy to understand yourself. If you dont see a specific variable in the wepon you're editing, try adding that variable. For example, dualies dodge number is based on the `RepeatCnt` variable. However, that variable only shows up on tetras. This is because it's left at the default value (2) for all other dualies. All you need to do in this case is add that variable in the same place and in the same way you see it on tetras.

This section will not cover everything you can do. Just some interesting things you can start with

### Ink Consumption
Down in the `WeaponParam` section for your weapon you will find a variable called `InkConsume` this variable tells the game how much ink to remove from the tank **per shot**.

### Paint Parameters
find a section called `PaintParam` these give you a ton of customization for how much paint the weapon does. Multiplying all the values by 10 gives you some really fun results.

### RNG
Down in the `WeaponParam` section for your weapon you will find multiple variables that start with `Jump_DegBias` and ` Stand_DegBias`. The Int values relate to how quickly (in frames) the RNG takes effect and the float values relate to how much RNG the weapon has in what situation (Jump or Stand)

### Range
At around line 18 where `MoveParam` is, find the variable called `SpawnSpeed`. While it might not look like it, this is range. The number represents range based on the weapon meaning something like inkbrush and 
 E-Liter will have similar values for this. Try not to think about it too hard. 

### Damage
Everything in `DamageParam` aside from `ReduceEndFrame` and `ReduceStartFrame`

### Fire Rate
Down in `WeaponParam` find the variable called `RepeatFrame` this tells the game to shoot a bullet every `X` frames 

### Homemade Aimbot
Up in `CollisionParam`, edit every variable that contains the word "Radius" to be maybe 50X larger. Also make sure that all of those values are the same. This increases the radius of your bullet's hitbox making it easier to hit targets as well as objects blocking the way.

# Class Specific Parameters

### Chargers - Increase Air Charge Speed

### Chargers - Force Scope, Divided Shots, and/or Charge Holding

### Dualies - Roll Count

### Dualies - Shoot while Rolling

### Dualies - End Lag

### Shooters - L-3 and H-3 Shooting (3 Shots)

### Splatanas - 1-Shot Radius

### Brushes - Rolling Ink Resistance

### Brushes - Roll Speed

### Blasters - Explosion Radius

### Splatlings - Recharge while Shooting

### Stringers - Charge Hold

### Stringers - Jump Tilt Angle

### Stringers - Trajectory Guide 

### Object Place Limit

# Misc

### Actor Swapping

### Weapon ID Swapping

### Ink Splatter Textures

### Stage Editing
Stage editing is pretty complex but right now, its not even possible with most of the stages. toolbox kinda dosent compile some of the byml files correctly so until thats fixed, dont worry about it

### Replacing Fonts


### Closing Notes


