```uml
@startuml

|__顧客__|
    :注文する;

|#AntiqueWhite|__販売部門__|
    :在庫を確認する;
    :出荷を確認する;

|__出荷部門__|
    :出荷する;
    fork
    :出荷を報告する;

|#AntiqueWhite|__経理部門__|
    :請求する;

|__顧客__|
    forkagain
    :商品を受け取る;

|__顧客__|
    end fork
    :支払う;

|#AntiqueWhite|__経理部門__|
    :入金を確認する;

@enduml
```
