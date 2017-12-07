## Weekly-GitHub-Digest #14
> 2017/11/30 - 2017/12/06

#### Web - 網路本身高風險，請詳閱公開說明書
- [makegirlsmoe/makegirlsmoe_web](https://github.com/makegirlsmoe/makegirlsmoe_web)  Create Anime Characters with MakeGirlsMoe
  
  > 這篇 AI 畫圖的[論文](https://makegirlsmoe.github.io/assets/pdf/technical_report.pdf)只能說太有愛了，選擇各種屬性和配置大頭貼就生出來了，相信用這些人物做為主角群編個劇本演部動畫會很有搞頭。自從 AlphaGo 在圍棋上展現了神乎其技的人類智慧結晶，各種相關的 Buzzwords 聲量都水漲船高，走在路上隨便找個人問你懂不懂 AI，相信都能說出大道理並不斷從中延伸，講到最後都像在談玄學，不過以筆者大學數理統計學重修的狀況，我想還是腳踏實地會好點，基礎數學底子都沒有的話大概就和小狗在汽車後頭追著跑一樣。
  <p align="center">
    <a target="_blank" href="https://github.com/makegirlsmoe/makegirlsmoe_web"><img alt="makegirlsmoe_web" src="https://i.imgur.com/WQc2lQc.png"></a>
  </p>
  
- [Jam3/math-as-code](https://github.com/Jam3/math-as-code)  a cheat-sheet for mathematical notation in code form
  > 指南也有人翻譯了[中文版](https://github.com/Jam3/math-as-code/blob/master/README-zh.md)，透過 JavaScript 適時的介紹各種數學符號，就算是當作複習也好。脫離學校生活之後，如果不是做相關研究工作的話應該會對數學越來越生疏，筆者連拿筆寫中文字都快有障礙了，更不用說更為精確複雜的數學運算，因此該是時候把過去的底子補上了，和技術債一樣，當你想要往更高的境界前進時，就會發現以前沒弄清楚的最後還是都要一ㄧ償還。
  <p align="center">
    <a target="_blank" href="https://github.com/Jam3/math-as-code"><img alt="math-as-code" src="https://i.imgur.com/AIeYhll.png"></a>
  </p>
---

#### Terminal - 已經是 iTerm 的形狀了呢
- [ismaelgt/metaweather-cli](https://github.com/ismaelgt/metaweather-cli)  ☀️ Command-line interface (CLI) for MetaWeather
  <p align="center">
    <a target="_blank" href="https://github.com/ismaelgt/metaweather-cli"><img alt="metaweather-cli" src="https://i.imgur.com/0WrVr5p.gif"></a>
  </p>
  
  
  > CLI 的花樣越來越多了，當初發明這介面的人真的是天才。有些東西在部分工程師眼裡或許過度本末倒置，例如原先的網頁應用已經足夠好用卻還是有開發者像是自虐狂般把 Twitter 或是 Facebook 搬到 CLI 呈現，不過像是畫圖看天氣這樣的應用就讓原本已經很潮濕的天氣顯得更潮了。結合了 MetaWeather 的資料，關於 ASCII arts 的圖示也參考了 [wego](https://github.com/schachmat/wego)，少了點炫目的轉場，輕量版的查詢天氣也是不錯玩：

  先來安裝一下：
  ```shell
  $ npm install -g metaweather-cli
  ```
  接著打：
  ```shell
  $ weather
  ```
  e04，選項好像沒有 Tainan，只好選唯一有的 Taipei：
  <p align="center">
    <a target="_blank" href="https://github.com/ismaelgt/metaweather-cli"><img alt="metaweather-cli" src="https://i.imgur.com/Bef9o3f.png"></a>
  </p>
  
  有時候真的覺得這些指令怎麼可以做得這麼簡單，打個幾行指令要的東西就蹦蹦跳出來了＠＠。
  
  至於天氣到底準不準就難說了 ( σ՞ਊ ՞)σ。
  
---

#### Useful OSS - 好用的開源軟體

- [Github Chrome Notifier](https://stacygohyunsi.github.io/)  Want to receive notifications for your Github repositories? Now you can. 

  > GitHub 本身的通知其實做的已經很不錯了，像是選擇 `watch` 即可觀察該專案的一舉一動，重要訊息從此不再 miss 掉，但如果像是有人 `star` 或是 `fork` 呢？也許有其他更為進階的使用方法，但就從目前的機制看來這部分並不是即時通知的，所以便有熱心的開發者跳出來嘗試解決這個問題了，只要簡單安裝它所提供的 [chrome extension](https://stacygohyunsi.github.io/usage/)，照著 README 走再輸入自己的 GitHub Name 便能成功啟用，筆者實際測試之後幾乎真的是 real time 的通知，可以試著玩玩看，btw，原作者也有在 [Medium](https://medium.freecodecamp.org/i-wanted-real-time-github-push-notifications-so-i-built-a-chrome-extension-7e6be0611e4) 上撰文描述製作的心路歷程，能夠把腦海中的點子做成實際可以運作的成品，就跟魔法一般神奇，我想這應該就是身為軟體工程師最大的熱情所在了。
  <p align="center">
    <a target="_blank" href="https://stacygohyunsi.github.io/"><img alt="Github Chrome Notifier" src="https://i.imgur.com/1b2yXO7.png"></a>
  </p>
---

#### Developers - 開發者們

- [Chris Wanstrath](https://github.com/defunkt)
  
  > 人們談論 Silicon Valley 往往只關注那些顯而易見的科技巨頭，FLAG 這樣的名詞你我都聽過，更不用說多少人拼命刷題擠破頭只為了搶得那張好像可以搭上高速列車的乘車券。你可能不會天天用 LINKEDIN 或是 Facebook，但做為一個還算敬業的工程師，瀏覽 GitHub 各種專案的頻率幾乎和多數人逛 porn sites 的次數差不多了，用這種比喻其實蠻糟糕的，但仔細想想還蠻貼切的。講了這麼多幹話，用意只在於 GitHub 平台是最容易被人忽略的，就跟陽光空氣網路一樣，它的工作如果做的夠出色基本上你是很難發現它有在運作的，但它確實很認真的在做事。Chris Wanstrath 做為另一個從大學休學的開發者兼任當前 CEO，在眾多有著同樣類似經歷和背景的科技名人這樣的歷史光環下，GitHub 從他口中的 side project 走向一個目前這個星球上最偉大的共享程式碼社群似乎也不是那麼天方夜譚了，而他本身這幾年雖然在平台上不怎麼活躍，但也不難發現像是 [jquery-pjax](https://github.com/defunkt/jquery-pjax) 這樣厲害的 repo 存在。可能很難再看到有這樣致力於開源也不斷支持並回饋社群的公司了。

---

#### Technical Posts - 你都去哪看技術文啊城武

- [vgod's blog](http://blog.vgod.tw/)
  
  > 踏入職場工作，到下禮拜也就滿一年了，筆者這陣子睡前都會花個二十分鐘，做類似冥想的思考，想想這一路上遇到的人事物和轉折，像是為何會跳入這巨大的坑等等，不過其中想最久的還是實習那段日子，當初會知道 IOH 就是因為看了 [vgod](https://ioh.tw/talks/%E9%BA%BB%E7%9C%81%E7%90%86%E5%B7%A5%E5%AD%B8%E9%99%A2-mit-%E5%BC%B5%E7%90%AE%E7%BF%94-vgod-chang-ov-study-phd-us/) 在上面的講談，而會知道 vgod 也是因為拜讀了他的[神乎其技系列](http://blog.vgod.tw/category/divine-code/)，和名字一樣，真的很神，某種程度和棋靈王有著同樣的魅力，就算是不會下圍棋的人同樣會被文中的描述所深深吸引。

---

#### You Need Some Music, And A Bottle of Dry Martini - 你一定要把氣氛搞得這麼銷魂嗎
- [Ai Otsuka - クムリウタ](https://www.youtube.com/watch?v=d0Pb-50oHGg&index=14&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op)
  
  > 一直到升大學的暑假才擁有人生的第一台筆電，也是自從那之後才比較常聽 JPOP 相關的樂團，電子樂 EDM 各種曲風都聽，但談到對於日本流行樂的啟蒙，絕對是大塚愛這個名字從腦海中蹦出，也是筆者相當欣賞的女歌手，那時高中在零用錢不多的情況之下還硬是跑去唱片行預購了當時剛出的精選輯，現在想來是完全值得的一次投資。創作型歌手不管放在哪個年代都會格外引人注目，是寶石總會發光的，加上她優異的鋼琴底子，這幾年的演唱會的模式變成全面自彈自唱，大獲好評的結果是必然的，衷心期待未來能夠再多來幾次台灣開唱。
  <p align="center"> 
    <a href="https://www.youtube.com/watch?v=d0Pb-50oHGg&index=14&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op">
      <img src="https://i.imgur.com/GEHTLvX.png" alt="Video Demo" />
    </a>
  </p>


---
> [關於作者](https://goo.gl/1pnqEk)

> [回到首頁](https://git.io/v5wk4)
