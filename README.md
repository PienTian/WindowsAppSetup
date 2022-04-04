# WindowsSetup
This powershell script is written for installing all primary apps into your newly windows computer.
You can add or drop applications by editing $pkgList.
when you add application, writing id form is recommended (you can check corresponding id by the command #winget search "app name"
make sure your network connection is enough fast.

このパワーシェルスクリプトは、windowsを新しくインストール,pcを新しく購入された方にお勧めです。
このパワーシェルスクリプトをダウンロードしてお使いください。
よく使われるアプリケーションが一気にインストールできます。
アプリケーションは　
$pkgListの中を編集することで好きなappを追加したり削除したりできます。id　形式がおすすめです。（winget search "探したいapp名")
気に入らないファイルがあればwinget uninstall "いらないapp"で消すことができます。
ネットワークがしっかりとつながるところでお試しください。

#FIXING BUG!
