
       spcmake_byFF6.exe
                                 　　　　      by pgate1

FF6サウンドドライバやFF6波形を使ってSPCを生成します。
MMLはFF6サウンドドライバ向けに特化したものです。

※警告
生成されるSPCにはFF6のサウンドドライバや波形データが含まれています。
SPCデータを容易に公開されることはご遠慮ください。


▼ 使い方

ご自身でFF6カートリッジからFinalFantasy6.romをダンプする。
FinalFantasy6.romをspcmake_byFF6.exeと同じ場所に置く。
必要であれば.brrを用意する。
sample.txt のようなMMLを書く。
spcmake_byFF6.batをダブルクリック。
エラーが無ければsample.spcが生成される。

・コツ

制御コードは16進大文字で 0x 等はつけない。
制御コードはスペースを空ける（実は開けなくてもよい）。
#toneは@の上であればどこで定義しても良い。
ノイズを使用する時はADSR設定のため何かしら波形を指定する必要あり。
「このファイルは"PKCS#7"として使用することはできません」のメッセージは.spcにプレイヤが関連付けられていないため。


▼ 履歴

2020/02/02
初版。


------------------------------------------------------------------------
@brr890様にはサウンドドライバやMML等について多くのアドバイスを頂きました。
心より感謝申し上げます。

SPCプレイヤには黒羽製作所様の黒猫SPCを使用させていただきました。
各レジスタ表示が分かりやすくデバグが捗りました。

SPCのデータ表示や解析にはVGMTransを使用させていただきました。
シーケンスや波形データ位置などの確認がし易かったです。

また次のサイトも参考にさせていただきました。先人の情報共有に感謝します。
・SuperC
　https://github.com/boldowa/SuperC-SPCdrv
・FinalFantasyVI 制御コード
　http://gnilda.rosx.net/SPC/F6/command.html
・FF6解析データ/サウンド ffbin@Wiki
　https://w.atwiki.jp/ffbin/pages/13.html


------------------------------------------------------------------------
pgate1
Web https://pgate1.at-ninja.jp
Twitter https://twitter.com/pgate1
