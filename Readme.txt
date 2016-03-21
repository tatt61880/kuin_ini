{
	Ini.kn v0.6 (for Kuin 1.01):
		Last Modified: 2016/03/21 23:21:14.
		Created by @tatt61880
			https://twitter.com/tatt61880
			https://github.com/tatt61880
}

【概要】
	1つのファイルに複数のデータを書き込めたら便利に違いない！
		→作成しました。

	Iniクラスを使用することで、複数のデータを1つのファイルで管理できます。
	ファイルの各行は以下のような構成になります。
		セクション名@キー名=値
	※Ini.knという名前ですが、Iniファイル形式と異なります。

【利用可能なクラス・メソッド一覧】
class CIni()
	func Init(filename_ :[]char) :Ini
	{文字列の保存・取得}
	func SetStr(sections_ :[]char, key_ :[]char, value_ :[]char) :bool
	func GetStr(sections_ :[]char, key_ :[]char, default_ :[]char) :[]char
	{数値(int型)の保存・取得}
	func SetInt(sections_ :[]char, key_ :[]char, value_ :int) :bool
	func GetInt(sections_ :[]char, key_ :[]char, default_ :int) :int

【更新履歴】
v0.60 2014/02/16
	[修正] Kuin 1.01で動作します。
v0.50 2013/10/19
	[修正] Kuin 1.00でコンパイルできるように修正しました。
v0.02 2013/05/04
	[変更] クラス名の先頭にはCを付けるようにしました。
	[修正] 動作する最低限のStdフォルダを追加しました。
v0.01 2013/04/28
	[初公開]

【参考】kndファイルは私の環境では下記に保存されていました。
	C:\Users\%USERNAME%\AppData\Roaming\MUP26ZR2TCP6KRT48EPSU6ZWBZKHJSMC
