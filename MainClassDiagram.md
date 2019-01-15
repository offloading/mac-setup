```uml
@startuml

title 主要クラス図

hide members
hide circle

class ヒト
class コト
class モノ
class 時
class 場所

ヒト <-- コト
モノ <- コト
コト --> 時
コト -> 場所

note right of ヒト : 個人/法人/部門...\n判断の主体

@enduml
```
