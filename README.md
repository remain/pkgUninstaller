# pkgUninstaller
## 説明
OS Xでは、.pkgからインストールしたアプリケーションにはアンインストーラが付属していないことが多く、アンインストールがとても不便です。
このRubyスクリプトは、OS X付属のpkgutilを用いてアプリケーションをアンインストールするものです。

## 注意事項
**実行には一部管理者権限が必要な部分があります。またファイル操作を行いますので、予期せぬシステムの破損やデータの消去が発生する恐れがあります。**
**テストは行っていますが、実行は自己責任でお願いします。**

## 使用方法
### –serach(-s)
パッケージのIDを検索します。部分一致で検索します。

### –unlink(-u)
インストールされたファイルとディレクトリを削除します。実行時はsudoと併用して下さい。

### –noop(-n)
–unlinkオプションと併用した時、ファイルとディレクトリの変更、及びパッケージ情報の削除を行いません。最後に削除されたファイル、ディレクトリ数を出力しますが、これは–noopオプション無しの実行と必ずしも一致しません。

### –quiet(-q)
–unlinkオプションと併用した時、削除されるファイルとディレクトリの名前、ディレクトリが空かどうかなどの情報を出力しません。削除されたファイル、ディレクトリ数は出力します。

### –help(-h)もしくはオプション無し
オプション一覧を出力します。

## 紹介記事
[Macでpkgからインストールしたアプリケーションを削除するpkgUninstallerを作りました](http://unasuke.com/howto/2014/how-to-use-pkguninstaller/)