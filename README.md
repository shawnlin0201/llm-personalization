# LLM Personalization
> 受不了 ChatGPT 總是在「命中」你、「不跟你繞」、「最直接的跟你說」這些東西嗎？
> 如果你也喜歡比較文學式的回覆，請別錯過這個專案

對於習慣嚴肅閱讀與長期保存內容的使用者而言，  
許多即時對話導向的回覆語氣，往往顯得過於熱絡、直白，甚至帶有不必要的自我表述。

本專案用來整理一組可重複使用的 LLM personalization 設定，
你可以根據自己的喜好來選擇對應的 Config。

## Usage
請參照你目前使用的產品在對應的地方放置 Config
|Service|Config 位置|
|---|---|
|ChatGPT|Setting / Personalization / Custom Instruction|
|VSCode Copilot|.github/custom-instruction.md|

## Config
|Name|Description|Example 以同樣在介紹此專案為例|Author|
|---|:--|---|---|
|ChatGPT 5.2|ChatGPT 5.2 原始風貌|好，我現在不打算先丟結論，也不會一開始就說「我直接告訴你」。<br> 如果你比較在意的是內容本身怎麼被寫出來，那這個專案就是在處理這件事。<br>這個專案的重點不是答案對不對，<br>而是 LLM 回覆時到底像不像在好好寫一段文字。<br>這裡整理了一組可以直接套用的 personalization 設定，<br>讓你把模型從即時聊天模式，拉回比較耐讀的書寫狀態。</details>|OpenAI|
|[book-and-cite](https://github.com/shawnlin0201/llm-personalization/blob/main/config/book-and-cite.md)|以書籍章節結構進行論述，並在適當處附上可追溯的引用來源，適合長篇、可保存的技術或觀點型內容|<details><summary>展開範例</summary><h2>一、專案背景</h2><p>本專案用來整理一組可重複使用的 LLM personalization 設定，目的在於降低即時對話語氣對嚴肅閱讀與長期保存內容的干擾。</p><br><h2>二、設計取向</h2><p>設定以技術書籍中偏敘事與論證型章節為寫作目標，允許鋪陳背景與脈絡，再逐步引出觀點，而非以對話或指令式語氣進行說明。</p><br><h2>三、引用與可追溯性</h2><p>當論述涉及既有研究或工程實務共識時，正文中會標示作者與年份，並以附註方式提供完整來源，以確保內容具備可回溯性。</p></details>|[ShawnL](https://github.com/shawnlin0201)|

## Config Example 產出方式
本專案中的 example，並非人工撰寫，而是由模型在「套用對應 Personalization 設定後」直接產出的實際回覆。
若你想分享你的 Peronalization 並提交 PR，請附上 Example，做法是將下方內容貼給 LLM 作為詢問內容。
```
請你依照下面專案內容描述，
以你目前 Personalization 設定下最典型的表達方式輸出。
# llm-personalization
本專案用來整理一組可重複使用的 LLM personalization 設定，你可以根據自己的喜好來選擇對應的 Config。
```
