# ロポコ(体験版)をMZ-700実機で遊ぶためのMZ-80K_SD差し替えプログラム

　Tookato様の素晴らしいゲーム「ロポコ(体験版)」をMZ-80K_SDを使ってMZ-700実機で遊ぶときのMZ-80K_SD用差し替えプログラムです。

　「ロポコ(体験版)」はMZ-80K_SDから起動は出来ますが、SDカードに対してセーブ、ロードはできません。

　そこでMZ-80K_SDのCMTモードをロポコ(体験版)モードに変更してSDカードに正常にセーブ、ロードが出来るようにするプログラムです。

　IPL-ROMにMZ-80K_SD用のパッチが当たっていれば「ロポコ(体験版)」には一切手を加える必要はありません。

　IPL-ROMを交換せずに「CMT2SD_CHECK」を使って「ロポコ(体験版)」にパッチを当てる方法も用意しました。

## 準備

### IPL-ROMにMZ-80K_SD用のパッチが当たっている場合
　ROMフォルダの「FD_rom_ROPOKO.BIN」を2764等のROMに焼き、MZ-80K_SDの通常のROMと交換します。

　SDカードに「ロポコ(体験版)」プログラムのMZTファイルを保存し、MZ-80K_SDに装着します。

### IPL-ROMにMZ-80K_SD用のパッチが当たっていない場合
　ROMフォルダの「FD_rom_ROPOKO.BIN」を2764等のROMに焼き、MZ-80K_SDの通常のROMと交換します。

　MZ-80K_SDレポジトリのCMT2SD_CHECKフォルダにある「CMT2SD_CHECK」を使って「ロポコ(体験版)」にパッチを当てます。

　SDカードにパッチを当てた「ロポコ(体験版)」プログラムのMZTファイルを保存し、MZ-80K_SDに装着します。

## 使い方
　MZ-80K_SDをSDモードに切り替えてロポコ(体験版)を起動します。

![SDモード](https://github.com/yanataka60/MZ-80K_SD_ROPOKO/blob/main/JPEG/SD%E3%83%A2%E3%83%BC%E3%83%89.JPG)

![ファイル選択](https://github.com/yanataka60/MZ-80K_SD_ROPOKO/blob/main/JPEG/%E3%83%AD%E3%83%9D%E3%82%B3(%E4%BD%93%E9%A8%93%E7%89%88)%E3%82%92%E9%81%B8%E6%8A%9E.JPG)

![LOADING](https://github.com/yanataka60/MZ-80K_SD_ROPOKO/blob/main/JPEG/LOADING.JPG)

　起動したらMZ-80K_SDをCMTモードに切り替えます。

![起動](https://github.com/yanataka60/MZ-80K_SD_ROPOKO/blob/main/JPEG/%E3%83%AD%E3%83%9D%E3%82%B3(%E4%BD%93%E9%A8%93%E7%89%88)%E8%B5%B7%E5%8B%95.JPG)

![CMTモード](https://github.com/yanataka60/MZ-80K_SD_ROPOKO/blob/main/JPEG/%E3%83%AD%E3%83%9D%E3%82%B3%E3%83%A2%E3%83%BC%E3%83%89(CMT%E3%83%A2%E3%83%BC%E3%83%89).JPG)

　後は、ロポコ(体験版)の説明書に従ってセーブ・ロードを行います。

　セーブデータはファイル名「ROPOKO.MZT」で保存されます。

　ロポコ(体験版)を遊び終わったらMZ-80K_SDをSDモードに戻すのを忘れないように。

　今回は、CMTモードのプログラムのみを修正しており、SDモードは従来通りです。CMTを使わない方はROMを差し替えたままでSDモードは従来通り使えます。

## 注意
　このプログラムをついてTookato様に問い合わせる等は絶対に行わないでください。

　このプログラムによりセーブデータが破損しても当方では一切責任は負えません。このプログラムの使用は自己責任でお願いします。

## 謝辞
　素晴らしいゲームを提供してくださったTookato様、ありがとうございます。

## 追記
2022.6.30

　アプリケーションからのロード、セーブをSD対応とさせるパッチあてWindows用ツール「CMT2SD_CHECK」に対応させました。

　「CMT2SD_CHECK」によりパッチを当てたロポコ(体験版)で遊ぶときにはMZ-80K_SDのROMを今回の「FD_rom_ROPOKO.BIN」に交換してください。