# object-oriented 5 design principle
># S: Single responsibility principle(SRP) 單一職責
>## 一個類別只負責一件事情

># O: Open/close principle(OCP) 開放/封閉原則
>## 要保留彈性，可以擴充新功能。改舊功能不影響新功能
>## 例:加裝雪鏈不需要整個輪胎換掉、更換燈泡不需要改棟引擎

># L: Liskov substitution principle(LSP) Liskov替換
>## 子類別應該可以替換掉父類別而不會影響程式架構
>## LSP談的是繼承，也就是透過繼承時子類別所造成的「行為變化」要如何設計
>## 子類別的實作必需可以替代父類別！也就是說父類別的實作必需在子類別也能運作。LSP和單一責任原則以及介面分離原則有很強的關聯
>## 例: 子類別樂高車無法執行父類別Car的「路上跑」功能

># I: Interface Segregation Principle(ISP) 介面隔離
>## 把不同的功能從介面中分離出來
>## 針對不同的客戶端，只開放其所需要的介面讓它使用，如此一來可避免與降低客戶端因為不相關介面改變也一起被迫需要改變的問題
>## 樂高車無法執跟其他子類超級跑車一樣執行「路上跑」的功能，所以就用介面將「路上跑」功能隔離出來

># D: Dependency Inversion Principle(DIP) 依賴反轉
>## 上層模組不應該相依於下層模組，而是隨時可以替換掉。
>## 相依於抽象或介面。而不相依於細節
>優點:
>1.可以隨時抽換掉，易於修改
>2.方便測試
>## 依賴反轉原則的目的是為了解除高階模組(People) 與低階模組(Hamburger) 的耦合關係，People 不再依賴 Hamburger ，而是兩者都依賴 Stuffer 介面
