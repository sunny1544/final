# Final Project README
## Build process
* 後端運用  

  * **`config.ini` 存放**  
  
    linebot 的 *Channel_Access_Token*、*Channel_Secret*  

    olami 的 *APP_KEY*、 *APP_SECRET*
  * **olami 對話訓練**
  
    ![image](https://user-images.githubusercontent.com/64915975/122667592-2b0eb700-d1e6-11eb-9546-5c55e2ee9d47.png)
  * **`girlfriend.py`為主要的main檔**，import `Flask` 、`Linebot`、 `nlp`等 相關套件，讓聊天機器人能運作
  * **新增 `__init__.py`** 為了讓 `girlfriend.py` import `nlp` 的時候認定 `nlp` 是一個 Module
  * **新增 `olami.py`** 實作 request OLAMI NLI API 的 method
  * **將程式部署到Heroku**  
    * **新增`Procfile`**，告訴Heroku如何啟動這個app
    * **新增`requirements.txt`**，告訴Heroku這個app的環境需要哪些其他套件
    * **新增`runtime.txt`**，告訴Heroku這個app指定的python版本
* 前端顯示、功能測試
  * **創建Linebot**

    ![image](https://user-images.githubusercontent.com/64915975/122666871-6b6c3600-d1e2-11eb-9706-857602094649.png)

  * **在Line Developer建立Linebot圖文選單**

    ![image](https://user-images.githubusercontent.com/64915975/122667035-4a581500-d1e3-11eb-99f3-91f956c2240e.png)
    
  * **對話測試**
 
    ![image](https://user-images.githubusercontent.com/64915975/122668529-0e28b280-d1eb-11eb-99dd-af507aa1c3ff.png)
## Introduction
* 主題發想來源：
近年來科技大幅進步卻也拉大了人與人之間的距離，生活步調日漸加速，與身邊人相處交心的機會卻也消逝減少；
部分人選擇了交友網站，卻敗給自己的不擅言詞，疫情期間也不能擅自外出遊樂，所以選擇製作出一款 LineBot 的虛擬女友。
* 目的：
給予使用者一個可以生動聊天、提供天氣預報、電影、音樂推薦還有簡單小遊戲的陪伴依靠
* 使用技術：
運用linebot結合NLP做出的聊天機器人。

  * 使用自然語言意理解處理(NLI)訓練機器人，讓機器人能更像真實人類回話。
  * 利用圖文選單，讓使用者有更簡單的操作。
  * 內涵天氣預報、推薦音樂和電影，讓使用者有更便利的生活。
  * 簡易的小遊戲讓使用者能夠度過無聊的時光。
* 使用流程：
![image](https://user-images.githubusercontent.com/64915975/122666323-298dc080-d1df-11eb-9a2c-6a5d65eccb1f.png)
## Details of the approach
## Results
## References
 1. Linebot NLP 結合+爬蟲 – 
  
    a. 實戰篇－打造人性化 Telegram Bot  
      https://zaoldyeck.medium.com/%E5%AF%A6%E6%88%B0%E7%AF%87-%E6%89%93%E9%80%A0%E4%BA%BA%E6%80%A7%E5%8C%96-telegram-bot-ed9bb5b8a6d9  
   
    b. （二）為 Chatbot 增加 NLP 功能  
      https://zaoldyeck.medium.com/%E5%88%A9%E7%94%A8-olami-open-api-%E7%82%BA-chatbot-%E5%A2%9E%E5%8A%A0-nlp-%E5%8A%9F%E8%83%BD-e6b37940913d  
    
    c. （三）為 Chatbot 添加新技能  
      https://zaoldyeck.medium.com/add-custom-skill-into-chatbot-cef9bfeeef52  
    
    d. Line Bot 助手機器人實作  
      https://skywalker0803r.medium.com/line-bot%E5%8A%A9%E6%89%8B%E6%A9%9F%E5%99%A8%E4%BA%BA%E5%AF%A6%E4%BD%9C-893e24db0ab5  
    
    e. [Python 網路爬蟲]YAHOO 電影-電影院,放映類型,放映時間(使用Yahoo API)  
      https://medium.com/@ethan.chen927/python%E7%B6%B2%E8%B7%AF%E7%88%AC%E8%9F%B2-yahoo%E9%9B%BB%E5%BD%B1-%E9%9B%BB%E5%BD%B1%E9%99%A2-%E6%94%BE%E6%98%A0%E9%A1%9E%E5%9E%8B-%E6%95%B8%E4%BD%8D-3d-imax-3d-%E6%94%BE%E6%98%A0%E6%99%82%E9%96%93-fc723e55727a

 2. olami 語法參考 -https://tw.olami.ai/wiki/?mp=osl&content=osl1.html
