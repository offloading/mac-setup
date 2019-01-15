```uml
@startuml
title パッケージ図と依存関係

' package
package 顧客 {}
package 受注 {}
package 商品 {}
package 在庫 {}
package 出荷 {}
package 請求 {}
package 回収 {}

' link
顧客 <. 受注
商品 <. 受注
受注 ..> 在庫
商品 <. 在庫
受注 <. 出荷
在庫 <. 出荷
出荷 <. 請求
請求 <. 回収
@enduml
```
