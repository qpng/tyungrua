## 中華拼音輸入法

### 前言

現代漢語同音字甚多。
若只按普通話讀音拼寫，在輸入法以及姓名、地名羅馬化上不甚方便。
何不利用各種方言取長補短，來從拼寫上區分更多的漢字？

爲此，固然可以使用基於中古《切韻》音系的拼寫法，但其分韻甚細之處，多數現代方言已不能區分。
所以刪其繁複，創作一個較簡潔的音系仍屬必要。
對古音、方言有興趣者，可以從本輸入法入門，在日常使用中增進對語言現象的理解。

本拼音方案詳見[此處][0]。
不過不必看完，即可開始嘗試打字。遇有不會的字，可按 ` 鍵用普通話反查。
本輸入法仍有大量細節待未來完善。
名稱亦是暫定，因「漢語拼音」一名爲普通話拼音所佔據，只好妄稱「中華」，莫譏太俗。

### 安裝

1. 本輸入法方案需要 [Rime 輸入法引擎][1]。

2. 將 `ime` 文件夾中的兩個 yaml 文件拷貝到 [Rime 的配置文件夾][2]（即該網頁上所稱的用戶資料夾）。

3. 編輯 Rime 配置文件夾中的 `default.custom.yaml`，[向 schema_list 中添加][3] `tyungrua` 一行。例如：

    ```
    patch:
      schema_list:
        - schema: luna_pinyin
        - schema: tyungrua
    ```

4. [重新部署][4]您的 Rime 輸入法引擎，然後按 Ctrl+` 打開方案選單，選擇「中華拼音」即可。


[0]: docs/tyungrua.md
[1]: https://rime.im/
[2]: https://github.com/rime/home/wiki/RimeWithSchemata#rime-中的數據文件分佈及作用
[3]: https://github.com/rime/home/wiki/CustomizationGuide#一例定製方案選單
[4]: https://github.com/rime/home/wiki/CustomizationGuide#重新佈署的操作方法