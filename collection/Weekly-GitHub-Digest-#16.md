## Weekly-GitHub-Digest #16
> 2017/12/14 - 2017/12/20

#### Web - 網路本身高風險，請詳閱公開說明書
- [Chalarangelo/30-seconds-of-code](https://github.com/Chalarangelo/30-seconds-of-code)  Curated collection of useful Javascript snippets that you can understand in 30 seconds or less
  
  > 大概是這一週以來最受歡迎的開源專案，筆者印象中就佔了 GitHub Trending JavaScript 類別的第一名有四天之久，不難想像這系列方釋出整個星星數就如同炸裂般往上暴衝，該 repo 收錄了非常多則簡短精悍的 JavaScript snippets，仔細看看，頂多兩三行左右不會最多的也不會超過五行，讓你透過最簡單的方式理解 JavaScript 這門語言各種新興特性和運作方式，對於 junior 或是 senior 都是不錯的研讀項目，其實看久了還蠻像 JavaScript Tips 的。不習慣看 GitHub README 的開發者，原作者也額外花時間整理並提供了一份更美觀更容易閱讀的[版本](https://chalarangelo.github.io/30-seconds-of-code/)，棒棒撻 🎉 ～
  <p align="center">
    <a target="_blank" href="https://github.com/Chalarangelo/30-seconds-of-code"><img alt="30-seconds-of-code" src="https://i.imgur.com/d63nOez.png"></a>
  </p>
  
- [croqaz/clean-mark](https://github.com/croqaz/clean-mark)  Convert an article into a clean text

  > 其實類似的服務已經蠻多的，但這個 repo 讀起來蠻容易實作的所以還是分享一下～。大致上就是透過 `global` 安裝的指令輸入文章的線上網址便能夠轉成指定的文件格式，支援 HTML，Markdown 等，有用的地方在於做一些文章收集時，許多人可能會連同圖片等不必要的廣告一同截入，藉由這個轉換器可以把文字部分單獨抽出，Markdown 的話筆者試用之後其實頗方便的，有關圖片的部份雖然就沒辦法這麼聰明了，但文章的基本資訊都能正確轉換，對做文章備份有格式潔癖的開發者們可以考慮玩一下。
  <p align="center">
    <a target="_blank" href="https://github.com/croqaz/clean-mark"><img alt="clean-mark" src="https://i.imgur.com/5iwrSul.png"></a>
  </p>
---

#### Terminal - 已經是 iTerm 的形狀了呢
- [briandennis/WebLauncher](https://github.com/briandennis/WebLauncher)  🌐 Easily open and manage website lists from the command line
  <p align="center">
    <a target="_blank" href="https://github.com/briandennis/WebLauncher"><img alt="WebLauncher" src="https://i.imgur.com/gdUihJh.gif"></a>
  </p>
  
  
  > 自從用了 Mac 之後 Chrome 的分頁越開越多，搞的才沒幾下子筆電就整個溫暖起來好棒啊，久了之後其實蠻惱人的，RAM 吃了一卡車之後只好改用 OneTab 管理分頁，但如果是遇上那種想要自由控制的分頁呢？像是每次開啟就會自動打開的幾個常用分頁，這樣的需求在 Chrome 自身的設定是可以做到的，但同樣的，對 CLI 控如我也是個不錯的嘗試：

  先來全域安裝一下：
  ```shell
  $ npm install -g web-launcher
  ```
  `web help` 來看看有哪些設定選項吧：
  ```javascript
  list [ls] 			           List all groups.

  groups    			           Add or remove a group.

  run [open] {groupName} 		 Open group in default browser.

  help    			             Print help menu.

  {groupName} 			         Run, add or remove sites from specified group.

  Key: [alias] {arg} ?{optionalArg}
  ```
  簡單舉例，如下操作可以在 local 端創建出一個名為 `dev` 的暫存空間：
  ```shell
  $ web groups -a dev
  ```
  然後把你要的網址塞進去：
  ```shell
  $ web dev -a youtube.com
  ```
  一個不夠用，再塞一個：
  ```shell
  $ web dev -a github.com
  ```
  通通打開吧！
  ```shell
  $ web dev open
  ```
  應該是慧根或能力值不夠，老實說我看了半天還是看不懂，最後還是透過那張 gif 才看懂配置，只能說，嗯。
  
---

#### Useful OSS - 好用的開源軟體

- [hql287/Manta](https://github.com/hql287/Manta)  🎉 Flexible invoicing desktop app with beautiful & customizable templates

  > 做 Invoice 設計的一項利器，介面不會過分華麗，主體配色相當自然且大方，配置設定也非常好上手，我特別喜歡原作者在 README 中提及的創作原因："The main reason I decided to build this is because I need a simple tool to create good looking invoices, estimates, and receipts but couldn't find one that suits my needs."。因為自己有這個需求但卻找不到合適的工具所以只好跳下來自幹了。所以那些處在問題當下的人果真是解決該問題的不二人選。
  <p align="center">
    <a target="_blank" href="https://github.com/hql287/Manta"><img alt="Manta" src="https://i.imgur.com/xCtL4Av.jpg"></a>
  </p>
---

#### Developers - 開發者們

- [Andrey Sitnik](https://github.com/ai)  Author of Autoprefixer, PostCSS and Logux
  
  > 近年人工智慧相關技術和新創公司如雨後春筍不斷冒出，矽谷有陣子大家的公司網域名都是什麼 `ＸＸＸＸ.ai`，但應該沒有什麼比 GitHub 帳號名就叫做 ai 要來的更潮的了 😎。著名的 PostCSS 原作者開源了為數相當驚人的專案，從做 easing function 參考時非常好用的 [easing.net](https://github.com/ai/easings.net)，幫你在 CSS 常見的屬性自動加上 prefix 處理的 [autoprefixer](https://github.com/postcss/autoprefixer)，又或者是產生測試用隨機 ID 的產生器 [nanoid](https://github.com/ai/nanoid)，幾乎可以很肯定的說你絕對用過他至少一到兩個甚至更多他所開發的工具。題外話，總覺得作者的頭像 icon 一直讓我聯想到光明會，是某種奇妙的反諷梗嗎？

---

#### Technical Posts - 你都去哪看技術文啊城武

- [Codepen Podcast](https://blog.codepen.io/radio/)
  
  > 關於技術部落格有誰說過一定要是純文字形式的呢？Podcast 也是一種極為出色的模式啊，國外已經紅了許久，充斥著更種選項，台灣有在做相關的似乎就少了蠻多，試想上了一整天滿滿八小時以上的班，身心疲憊之餘只想好好睡個覺補個眠，雙眼乾澀到不行之後回家繼續用筆電上網實在是痛苦不堪，更不用說長期累積下來出現的煩人飛蚊症和黃斑病變，與其如此自討苦吃倒不如嘗試在下班之後用耳朵聽聽 Podcast，培養成習慣之後既紓壓又自在，其實是極容易上癮的，尤其 Codepen 提供的內容取材甚廣沒話說，訪談同時兼具深度廣度，從現在開始的下班時間讓眼睛好好休息吧。

---

#### You Need Some Music, And A Bottle of Dry Martini - 你一定要把氣氛搞得這麼銷魂嗎
- [Pay Money To My Pain - Home](https://www.youtube.com/watch?v=R-X6I5sRfyo)
  
  > Pay Money To My Pain 團名取的很棒，更多人會用 P.T.P.稱呼他們，第一次接觸的人建議可以看看 [KAZBOM](https://www.youtube.com/watch?v=_87GLJJnCqI) 所製作的樂團介紹，就算之前沒聽過看了會感到想哭也是挺正常的，之前他們也曾和 ONE OK ROCK 合作過 [VOICE](https://www.youtube.com/watch?v=8wTm9ouWrTo) 這首歌，同時也收錄在 P.T.P. 成團以來所出過的最後一張專輯。熟悉第一神拳的人也絕對聽過他們的 [Weight of My Pride](https://www.youtube.com/watch?v=eqfDSb648g8)，看鷹村痛扁 Hawk 搭上主題曲整個熱血。P.T.P. 可以說代表作無數，只是離去的太突然，這段演出是在主唱 K 因心臟衰竭離世之後剩餘團員所做的紀念演唱會，舞台中央的麥克風位置空無一人，燈始終聚光在那。
  <p align="center"> 
    <a href="https://www.youtube.com/watch?v=R-X6I5sRfyo">
      <img src="https://i.imgur.com/UbOiYyu.png" alt="Video Demo" />
    </a>
  </p>


---
> [關於作者](https://goo.gl/1pnqEk)

> [回到首頁](https://git.io/v5wk4)
