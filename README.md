# WindowsSetup
This powershell script is written for installing all primary apps into your newly windows computer.
You can add or drop applications by editing $pkgList.
when you add application, writing in id form is recommended (you can check corresponding id by the command `winget search "app name"`
make sure your network connection is enough fast.

このパワーシェルスクリプトは、windowsを新しくインストール,pcを新しく購入された方にお勧めです。
このパワーシェルスクリプトをダウンロードしてお使いください。
よく使われるアプリケーションが一気にインストールできます。
アプリケーションは　
$pkgListの中を編集することで好きなappを追加したり削除したりできます。id　形式がおすすめです。（`winget search "探したいapp名"`)
気に入らないファイルがあれば`winget uninstall "いらないapp"`で消すことができます。
ネットワークがしっかりとつながるところでお試しください。



## If You Can't Run Powershell Script
copy & paste or type following commands to your powershell and run as admin (win+R to open launcher and type powershell, then hold ctrl+shift and hit enter key)

アドミニストレータとしてpowershellを起動し(win+R, powershellと入力,ctrl+shift+enter key, はいを選択)
以下のコマンドをコピーペーストまたはタイプしスクリプトを実行可能にしてください

**`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned`**
and then

**`Unblock-File -Path /Path/to/WindowsSetup`** or 

`Get-ChildItem -Path C:\ -Name WindowsSetup.ps1 -Recurse | ForEach-Object {"C:\$_"} | Get-Item | Unblock-File`



>*if still you can't run, please try loosing execution policy.*

>*`Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted` (not recommended)*
*or copy paste as new psm1 and psd1 file.*

>_それでも動かなかった場合は、上記のコマンドでポリシーを緩めるか、.ps1ファイルを新しく作成して内容をコピペしてください。_


### If you don't install Alacritty
you don't need to setting up alacritty, thus after `foreach` block, you can delete all the code and it's prefered :)

Alacrittyをインストールしない場合は`foreach`ブロック以降のコードを削除することをお勧めします。

### Execution
right click WindowsSetup.ps1 and choose 'Run with PowerShell'

WindowsSetup.ps1ファイルを右クリックしPowerShellで実行を選択。
