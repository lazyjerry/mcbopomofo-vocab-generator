# 小麥注音詞語產生器

這是一個用於生成符合小麥輸入法自訂詞彙格式的網頁工具。透過本工具，你可以快速產生「詞 語音」格式的資料，其中注音音節自動轉換並以 `-` 分隔，方便直接複製至小麥輸入法的自訂詞彙檔案中。

## 功能特點

- **自動注音轉換**  
  輸入中文詞語後，工具會利用 [zhuyin87](https://github.com/signxer/zhuyin87/tree/master) 套件自動將文字轉換成注音，並將空白替換為 `-`，滿足小麥輸入法的格式需求。

- **多筆資料輸入**  
  每次點擊「生成詞彙」後，產生的結果會追加到結果區塊中，並自動清空輸入欄位，以便連續添加多筆詞語。

- **Bootstrap 5 美化**  
  使用 Bootstrap 5 框架實作現代化、響應式的使用者介面。

## 使用方式

1. **Clone 此倉庫**  
   ```bash
   git clone https://github.com/yourusername/mcbopomofo-vocab-generator.git
   cd mcbopomofo-vocab-generator
	```

2. 檢查依賴
- 請確認已下載或引入 zhuyin87 套件。
- 此專案同時需要 pinyinUtil.js、zhuyinUtil.js 以及相關的字典檔（pinyin_dict_notone.js 與 pinyin_dict_withtone.js），請確保這些檔案位於正確的路徑下（例如：./dict/）。
3. 運行專案
- 直接在瀏覽器中開啟 index.html（或專案中相應的 HTML 檔案），即可使用此詞語產生器。

## 文件格式

生成的詞語格式符合小麥輸入法自訂詞彙檔案的要求，每筆詞語的格式如下：

中文詞語 注音

其中，注音部分必須將每個注音音節以 - 分隔，例如：

小麥注音 ㄒㄧㄠˇ-ㄇㄞˋ-ㄓㄨˋ-ㄧㄣ

將生成的結果直接複製並貼入小麥輸入法的自訂詞彙資料檔中即可。

## 參考與相關資源
- zhuyin87
https://github.com/signxer/zhuyin87/tree/master
使用此套件進行中文轉注音並進行格式化處理。
- 小麥注音官網
https://mcbopomofo.openvanilla.org/
官方網站提供小麥輸入法相關資訊與下載。
- 小麥輸入法自訂詞彙使用手冊
https://github.com/openvanilla/McBopomofo/wiki/使用手冊#手動加詞

## Demo

線上 Demo 網頁: https://mcbopomofo-vocab-generator.pages.dev/

## License

本專案採用 MIT 授權，歡迎參考與修改。

## Contributing

如果你對此工具有任何疑問或建議，歡迎提交 Issue 或 Pull Request，一起讓這個詞語產生器變得更好！
