# Awesome-Splatoon3-Hacking
[DesperC](https://github.com/DesperC)によるスプラトゥーン3のハッキング/改造を学ぶためのリソースが入った非公式日本語版Repo

このレポは巨大なW.I.P.であり、非常に未完成です。このRepoはDesperCによるサイドプロジェクトです

もしあなたが行き詰まったり、助けが必要だと感じたら、[Splatoon Modding Hubディスコードサーバー](https://discord.com/invite/P6RNNvk)に気軽に参加してください

この内容は殆ど古いので、まだ何か必要なら上のサーバーに参加して助けを求めてください

オンラインでのMod/ハックの使用方法を教えるものではありませんし、オンラインでの使用は安全ではありません。後でバトルリプレイでのカメラハックの使用に関するセクションがあるかもしれませんが、それだけです。これらをオンラインで使用せずに、改造されたSwitchを正しくセットアップしてください


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
- セーブデータのエクスポート、編集、インポート
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

以下は、ゲームの特定の側面を置き換えるために必要なプログラムに関するサブセクションです。***これは、改造可能な全てのもののリストではありません。あくまで、特定の改造に必要な他のプログラムのリストです***

### テクスチャの置き換え（旧）
- Hex Editor. どんなHex Editorでもいい。個人的には [HxD](https://mh-nexus.de/en/)
- Image Editor (Duh)
- [Blender](https://www.blender.org/) テクスチャがモデル上でどのように見えるかを確認する

### テクスチャの置き換え
- Image Editor (still, duh)
- [Blender](https://www.blender.org/) テクスチャがモデル上でどのように見えるかを確認する

### モデルの置き換え
- [Blender](https://www.blender.org/) または他の3Dエディターとその使い方の知識が必要です。基本的に3Dモデルの経験が必要です

### Text Replacement
- [Kuriimu](https://github.com/IcySon55/Kuriimu) または [Kuriimu 2](https://github.com/FanTranslatorsInternational/Kuriimu2)
Kuriimu 2はより永続的なインストール方式であり、Kuriimuは軽量でポータブルなソリューションです

### Audio Replacement
- [Looping Audio Converter](https://github.com/libertyernie/LoopingAudioConverter)
- [Citric Composer](https://gota7.github.io/Citric-Composer/)
- [Automatic BARS Patcher](https://github.com/ic-scm/automatic-bars-patcher) or [Online BARS Patcher](https://smashcustommusic.net/onlinetools/bars-patcher/)
- [Foobar2000](https://www.foobar2000.org/) + [VGMStream](https://www.foobar2000.org/components/view/foo_input_vgmstream)
- Audio Editor. 個人的には [Audacity](https://www.audacityteam.org)

# RomFSのダンプ

### エミュレータ (初心者推奨) (Switchを使用しない場合は必須)
（インストールしたいアップデートやDLCがある場合は、NSP形式でインストールしてください）ゲームを右クリックし、「RomFSをダンプ」を選択します。**これらのファイルをどこにダンプしたかを必ず覚えておくか、覚えやすい場所に置いておいてください**

### Switch（初心者向けではない）
Lockpick_RCMとNxdumptoolが必要

Lockpick_RCMへのリンクは許可されていませんが、Githubの多くの場所で見つけることができます

その後、この[動画](https://www.youtube.com/watch?v=mKw2ips97og)を見て使い方を学びます

それが終わったら、(Nxdumptoolのnroファイル)[https://github.com/DarkMatterCore/nxdumptool/releases]をダウンロードします

次に、この(動画)[https://www.youtube.com/watch?v=BZpK2JT8lcI]を見てそれの使い方を学びます

私が自分で説明しない理由は、このガイドがゲームの改造に焦点を当てているためで、セットアップについては説明していないからです

