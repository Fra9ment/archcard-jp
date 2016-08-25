#概要
これらの簡単なスクリプト・画像は名刺を生成するためのものです。
出力形式はSVGで統一しているので、高品質な出力が得られます。
背面用画像も用意してあります。

#依存関係
Arch Linuxでのパッケージ名に準拠しています。
##依存
* python(ただし、Python 3)

##推奨(表示・印刷時の正確性に関係)
* otf-ipafont
* noto-fonts
* noto-fonts-cjk

#構成
##ファイル類

###/dialog2card.py
ダイアログ形式で名刺を生成するスクリプト。これが使えれば基本動作は十分です。  
名前(と出力ファイル名)と役職を聞いてきます。  

**注意**として現在は**.png**以外は使えない仕様です。

###/mods.py
他のファイルからimportするためのファイルです。
頻繁に使うような煩雑なスクリプトをまとめます。  
例) GEN関数(テンプレートから名刺を生成)

###/template.svg
このファイルをスクリプトで編集、出力します。

##ディレクトリ

###/output/
このフォルダに名刺が吐かれます。

###/pics/
プロフィール画像を収めます。  
'**YOURNAME**.png'というファイル名(YOURNAMEは所持者の名前)で、縦横比は1:1を推奨

###/back/
背面用の画像が収められています。
間違ってもバックアップ用ではありません。

###/edit/
大差はないですが、テンプレート出力前のInkscapeでの編集ファイルが入っています。  
(ガイドの有無等の差があります。)
