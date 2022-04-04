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

now it works!:)
動きます(..

### If You Can't Run Powershell Script
copy & paste or type this command to your powershell and run as admin (win+R to open launcher and type powershell, then hold ctrl+shift and hit enter key)

アドミニストレータとしてpowershellを起動し(win+R, powershellと入力,ctrl+shift+enter key, はいを選択)
このコマンドをコピーペーストまたはタイプしスクリプトを実行可能にしてください

 Set-ExecutionPolicy -ExecutionPolicy RemoteSigned
 
