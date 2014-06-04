# 程式： YouTube 影片下載器

## 使用方法

使用者輸入下載指令，第 1 個參數是下載影片存檔的名稱，第 2 個參數是 YouTube 網址。

```
java -jar VideoDownloader.jar [filename] [youtube-url]
```

## 此程式流程如下：

1. 利用第三方工具 [Selenium](http://docs.seleniumhq.org/) 的 HtmlUnitDriver 類別，操作 [Kej's FLV Retriever](http://kej.tw/flvretriever/) 以取得 YouTube 的靜態下載連結
1. 在目錄 .hisdir 下建立傳輸歷史檔、下載檔案
1. 將下載完成的檔案，搬移到 [filename]
