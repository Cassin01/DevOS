# DevOS
坂井弘亮 12ステップで作る組み込みOS自作入門備忘録

## キーボードレイアウト変更

```shell
loadkeys us
```

## パスワード

(一般ユーザ) ID:user Password:progtooluser

(スーパーユーザ) ID:root Password:progtoolroot

## 参考

http://tkygtr6.hatenablog.com/entry/2018/02/25/201410

少し参考書と違うところがある(単純な間違いと思われる。)
h8writeディレクトリがないので作る。

## 注意事項

- make writeはsuでないと実行できない。

## minicom

- シリアルファイルはminicomを使用する場合``/dev/serial/by-id/usb-FTDI_USB_Serial_Conveter_FTEFGBJ1-if00-port0``だと長すぎる為記述できない。代わりに``/dev/ttyUSB0``が使用できる。

- ``minicom -s -o`` で設定画面起動

- ``minicom -o`` で通常起動

- ``C-a s`` で転送ファイル指定

- ``C-a x`` で終了

## リンカスクリプトについて

以下が参考になった

[リンカスクリプトの書き方](http://blueeyes.sakura.ne.jp/2018/10/31/1676/)
