# 學習測試

![](http://continuousdelivery.com/images/test-quadrant.png)
(圖片來自：http://continuousdelivery.com/foundations/test-automation/)

## 業務導向且支持開發過程的測試

### 驗收測試
- 確保用戶故事的驗收條件得到滿足
- 做對的事情 (the the right thing)
- 由用戶寫測試腳本，開發人員和測試人員努力實現這些腳本
- Happy Path: Given-When-Then
- 自動化驗收測試
  - 加速反應速度
  - 減少測試人員負擔
  - 提高探索性測試與高價值的活動
  - 支援回歸測試
  - 活文件 (不斷更新的規格書)

## 技術導向且支持開發過程的測試

### 單元測試
- 單元測試單獨測試一段特定的程式碼
- 把事情做對 (do the thing right)
- 常常倚賴測試替身 (test double) 模擬系統其他部分
- 沒有系統組件間的交互，執行速度快
- 偵測修改程式碼是否破獲現有的功能

### 組件測試
- 用於測試功能集合，捕捉系統不同部分交互產生的缺陷
- 需要執行更多 I/O 操作、連接資料庫、檔案系統等

### 部署測試
- 用於檢查部署過程是否正常
- 應用程式是否是否正確安裝、配置，能否與所需的服務連接，得到相對的回應

## 業務導向且評價專案的測試

### 展示
- 每次迭代結束時，敏捷開發團隊向用戶展示其開發完成的新功能
- 頻繁地向客戶演示功能，儘早發現對需求規格的誤解，或修正有問題的規格

### 探索性測試
- 創造學習的過程，不只是發現缺陷
- 創建新的自動化測試，用來覆蓋新的需求

### 易用性測試
- 驗證用戶能否容易使用軟體完成工作
- 情境調查：觀察使用者操作過程，收集量化數據，如使用者多久時間完成任務、按了多少次錯誤的按鈕、試用者自評滿意度
- Beta測試：網站同時運行多個版本，收集、統計、分析新功能的使用情形，讓功能適者生存不斷演進

## 技術導向且評價專案的測試

### 非功能性測試
- 除了功能之外的系統品質測試，如容量、可用性、安全性
- 客戶不關心非功能需求，但當他們意識這方面的問題，事情往往一發不可收拾
  - 容量：網站因為容量問題，停止提供服務
  - 安全性：用戶個資外洩、信用卡被盜刷

## 開發流程
- 客戶、分析師、測試人員**定義**驗收條件
- 測試人員與開發人員基於驗收條件，**實現**驗收測試自動化
- 開發人員編寫程式**滿足**驗收條件
- 只要有自動化測試失敗，無論是單元測試、組件測試、驗收測試，開發人員要優先處理並修復問題

## 參考資料
- [Continuous Testing](http://continuousdelivery.com/foundations/test-automation/)
- [Behavior-Driven Development in Python](http://code.tutsplus.com/tutorials/behavior-driven-development-in-python--net-26547)
- [behave](http://pythonhosted.org/behave/) is behaviour-driven development, Python style.
- [Lettuce](http://lettuce.it/) is a Behavior-Driven Development tool written by Gabriel Falcão G. de Moura.
- [unittest](https://docs.python.org/3/library/unittest.html) — Unit testing framework
- [unittest.mock](https://docs.python.org/3/library/unittest.mock.html) — mock object library
- [unittest.mock-examples](https://docs.python.org/3/library/unittest.mock-examples.html) - getting started
- [Doubles](http://doubles.readthedocs.io/) is a Python package that provides test doubles for use in automated tests.

