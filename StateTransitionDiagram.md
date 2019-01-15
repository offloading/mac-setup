@startuml

title 状態遷移図の例
skinparam shadowing false

state 審査中
state 承認済
state 実施中
state 中断中
state 差し戻し中
state 終了

[*] --> 審査中 : 申請
審査中 --> 承認済 : 承認
承認済 --> 実施中 : 開始
実施中 --> 中断中 : 中断
中断中 --> 実施中 : 再開

審査中 -> 差し戻し中 : 差し戻し
差し戻し中 -> 審査中 : 再申請
差し戻し中 -down-> 終了 : 取り下げ

承認済 --> 終了 : 取り下げ
実施中 --> 終了 : 完了
中断中 --> 終了 : 中止

終了 --> [*]

@enduml
