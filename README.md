◆概要

秋月ジャンクマトリクスLEDを Arduino UNO で動作確認するプログラム

- 起動後に１６ｘ１６ドットの塗りつぶしパターンがモジュール右側から左側へ移動を繰り返す

- 以下に記すボタンを用意し、このボタンを押下することで表示パターンを以下の順で変更する

　- １６ｘ１６ドットの塗りつぶしパターン

　- 横線＋斜め線のパターン

　- １６ｘ１６ドットフォントの「赤」

マトリクスLEDモジュールは１セットでの使用を想定

なお、動作確認は Cytron社の Maker UNO を使用

https://akizukidenshi.com/catalog/g/g116285/

https://www.cytron.io/p-maker-uno-simplifying-arduino-for-education?search=MAKER-UNO&description=1

◆参考資料

https://akizukidenshi.com/img/contents/kairo/%E3%83%87%E3%83%BC%E3%82%BF/%E8%A1%A8%E7%A4%BA%E8%A3%85%E7%BD%AE/LED%E9%9B%BB%E5%85%89%E6%8E%B2%E7%A4%BA.pdf

◆参考情報１

Maker UNOの回路図

https://cdn.cytron.io/makeruno/MAKER-UNO.pdf?_gl=1*1eylfr3*_gcl_au*MTk1OTE4MzI1Ny4xNzQwMzc2Mjg5

◆参考情報２

https://x.com/YI_Studio/status/1842111760213663799

https://x.com/YI_Studio/status/1893488568930025907


◆ピンアサイン

マトリクスLEDモジュールと接続するピンは以下の通り。

#define SIN1PIN         3

#define SIN2PIN         4

#define SIN3PIN         5

#define CLKPIN          6

#define LATPIN          7

また、表示内容の変更に使用するボタンのピンは以下の通り。

#define BTNPIN          2

※ボタン押下時にGNDへ接続される想定。

![schem](https://github.com/Y-Ishioka/UNO_junk_test/blob/main/btn_pin.jpg)


◆免責

　著作者は，提供するプログラムを用いることで生じるいかなる損害に関して，一切の責任を負わないものとします．

　たとえ，著作者が損害の生じる可能性を知らされていた場合も同様に一切の責任を負わないものとします．
