## 介紹前端框架中-angular.js
### 為什麼要介紹angular.js?
* 與Typescript做連結，應用到實際層面

* 前端語法結合PHP，讓程式碼更為整潔

### Typescript做連結是哪一個方面?

>Typescript的好處不只在型別檢查，而是<b>物件導向</b>方式，讓團隊在開發大型專案上更為容易，不用額外註解太多也能理解團隊其餘成員所做的動作。
### 起因 : 想讓物件導向的概念執行在專案上

>想利用TS寫常用的FUNCTION，利用HTML引入的方式，讓專案上常用的部分都能包成一個模組。

### 失敗 : TS的FUNCTIOIN無法有效與HTML做結合

>嘗試TS的export和html的import還沒找到好方法做完美連結

## 救星出現-angular.js出現

### angular.js環境建置
1. html文件引入angular.js
`<script>https://cdn.staticfile.org/angular.js/1.6.3/angular.min.js</script>
`
2. 設置ng-app屬性   
必須要在你的HTML中設定ng-app屬性，例如：`<html ng-app>`AngularsJS 看到 ng-app 後就會自動初始化該標籤範圍內的程式
3. 設置ng-controller    
`<div ng-controller="MsgController">`   
此處為Controller控制的範圍
4. `script範圍內`   
首先建立一個自訂的 module 叫做 ModuleA  
`var moduleA = angular.module("ModuleA", []);`
再來設置要使用的modle下的Controller
`moduleA.controller("MsgController", [function() {this.Message = "測試一下";}]);`

### 以下DEMO有關於Angular.js ajax的部分












 