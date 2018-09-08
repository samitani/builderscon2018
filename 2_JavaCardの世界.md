## Speeker

## Java Card
* SIM/Credit Card etc..
  * B-CASも？

* SmartCard
 * ISO 7816
 * Intelligent Smart Card - CPUが乗ってる
 * クレカの金色のチップ部分で外部と通信
    * APDUというプロトコル
 * Java CardはSmart Cardの一種

* Application Protocol Data Units

* UICC Universal Integrated Circuit Card
  * ある程度の演算処理が可能

* Java Card
  * short / byte ぐらいしか使えない、int / float / double はない

* セキュリティ
  *　Applet どうしは隔離されてる
    * 明示的に共有するデータは指定できる
  * インスタンス変数はEPROMに書き込まれる
    * 電池が切れてもデータは残る
    * 同様に、JVMも動き続ける（電源が復活したら、止まったところから動作再開）
  * RAM
    * 8バイトしかない・・・
    * 奪い合いになる