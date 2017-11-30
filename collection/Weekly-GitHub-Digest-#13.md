## Weekly-GitHub-Digest #13
> 2017/11/23 - 2017/11/29

#### Web - 網路本身高風險，請詳閱公開說明書
- [coltaemanuela/FireEdit](https://github.com/coltaemanuela/FireEdit)  🔥 FireEdit is a real-time text editor which allows programmers work simultaneously
  
  > 數十年前曾發生過 Vim 和 Emacs 的編輯器大戰，每次看到國外網友在吵這個都覺得意味不明，把講幹話的時間拿來投資在其他地方充實自己不是會更有生產力嗎？現在的開發者在選擇上比起以前也多了不少選項，介面美觀大方的 Atom，穩定好棒棒經典款 Sublime，還有近期越來越多人使用的 VSCODE，也可以觀察到像是 [teletype](https://github.com/atom/teletype) 和 [live-share](https://code.visualstudio.com/blogs/2017/11/15/live-share) 這樣 real-time 的協作工具的陸續出現勢必會帶來更多的便利性，這回介紹的 FireEdit 功能上雖然陽春許多，但基本協作功能還是有的，使用了 Firebase 這點也不難看出，開發這項作品的原作者也寫了篇[簡介文](https://www.codementor.io/johnnyb/fireedit-real-time-editor-javascript-firebase-59lnmf3c6)說明，程式碼其實不到特別多，花些時間細讀相信會有所收穫的。
  <p align="center">
    <a target="_blank" href="https://github.com/coltaemanuela/FireEdit"><img alt="FireEdit" src="https://i.imgur.com/6juwwos.png"></a>
  </p>
  
- [edent/SuperTinyIcons](https://github.com/edent/SuperTinyIcons)  Under 1KB each! Super Tiny Icons are miniscule SVG versions of your favourite website and app logos
  > 分享 Icon 類的 repos 似乎有越來越蓬勃的跡象，像是收集了大大小小常見圖示也非常佛心開源的 [feather](https://github.com/feathericons/feather)，加上今天介紹更為專注在收集網站和一些常用 App 圖示的 SuperTinyIcons，雖然不到包山包海的程度，但較為主流的幾個 logo 也不難找到，像是 Medium，GitHub，Steam，連筆者很少用的 LINE 也有，看 repo 更新的速度應該還是在持續更新中。
  <p align="center">
    <a target="_blank" href="https://github.com/edent/SuperTinyIcons"><img alt="SuperTinyIcons" src="https://i.imgur.com/fySszOS.png"></a>
  </p>
---

#### Terminal - 已經是 iTerm 的形狀了呢
- [SBoudrias/Inquirer.js](https://github.com/SBoudrias/Inquirer.js)  A collection of common interactive command line user interfaces
  <p align="center">
    <a target="_blank" href="https://github.com/SBoudrias/Inquirer.js"><img alt="Inquirer.js" src="https://i.imgur.com/hQWkUkh.gif"></a>
  </p>
  
  
  > 事實上很多東西只要把同樣的畫面搬到 CLI 的介面上呈現，總是會讓人覺得哇～好像挺讚的，但難度就在於這件事情並不是這麼容易被實踐，好在身處今日的我們有了各種神奇的工具，可以有效的站在巨人的肩膀上看的更高更遠，製作 CLI 相關工具的難度可以說降低非常多，原本這系列想好好打包來個鐵人賽 30 天自我挑戰，但原諒筆者如果再持續這樣的生活模式下去還沒變成鐵人就先肝硬化了，還是想留點和自己對話的時間，反正同樣是寫作嗎嘻嘻 ʕ•͡ᴥ•ʔ。回到正題，你可能在安裝許多 npm package 時看到這種互動式的選項，每個選擇都會導向不同的結果，其實大多數的邏輯都有辦法藉由 Inquirer 這套做出來：

  首要之務當然是先安裝一下：
  ```shell
  $ npm install inquirer
  ```
  雖然 README 寫的挺詳細的，但筆者更推薦直接看 example folder 下的例子更快更直接：
  ```javascript
  var questions = [
    {
      type: 'confirm',
      name: 'toBeDelivered',
      message: 'Is this for delivery?',
      default: false
    },
    {
      type: 'input',
      name: 'phone',
      message: "What's your phone number?",
      validate: function(value) {
        var pass = value.match(
          /^([01]{1})?[-.\s]?\(?(\d{3})\)?[-.\s]?(\d{3})[-.\s]?(\d{4})\s?((?:#|ext\.?\s?|x\.?\s?){1}(?:\d+)?)?$/i
        );
        if (pass) {
          return true;
        }

        return 'Please enter a valid phone number';
      }
    },
    {
      type: 'list',
      name: 'size',
      message: 'What size do you need?',
      choices: ['Large', 'Medium', 'Small'],
      filter: function(val) {
        return val.toLowerCase();
      }
    }
  ]
  ```
  上面拿的是 `pizza.js` 這個範例做為教學，簡單的幾條程式碼就看到了輸入驗證，選擇題等操作方式，應該可以感受到這項工具的強大以及易用性了吧！其他還支援了 checkbox，input 資料輸入時的讀取都應有盡有，腦海頓時冒出超級多可以延伸的相關應用，Inquirer 真的非常有魅力。
  
---

#### Useful OSS - 好用的開源軟體

- [chinchang/web-maker](https://github.com/chinchang/web-maker)  A blazing fast & offline frontend playground 

  > 自從用過 Codepen 之後就很難再找到類似夠格打對台的產品，畢竟 Codepen 已經支援了多項 preprocessor，前端各種能玩的把戲都能在上面找到，也越來越多教學類的展示轉往這個戰場，就是因為它太簡單太好用太容易上手了，開源圈是否也有著類似的專案呢？Web-Maker 或多或少能夠滿足你的想像，筆者個人的習慣是，如果只是想單純測試並且驗證一個簡單的 PoC，另外在 Codepen 多開一個瑣碎的專案實在很不必要，所以我更會選擇直接裝 Web Maker 的 browser extension，使用後的感受其實挺直接的，加上它在 offline 時同樣可以正常運作，某些情境下能夠多些這樣的替代工具其實也間接讓選項變得彈性許多。
  <p align="center">
    <a target="_blank" href="https://github.com/chinchang/web-maker"><img alt="eb-maker" src="https://i.imgur.com/00VObhf.png"></a>
  </p>
---

#### Developers - 開發者們

- [Jorge Bucaran](https://github.com/jorgebucaran)
  
  > Jorge Bucaran 是前陣子讓筆者感到極為驚艷的 [hyperapp](https://github.com/hyperapp/hyperapp) 作者，這是一個總大小僅約 1KB 左右的前端 library，同樣是基於 VDOM 本身，API 的整體設計乍看之下有點像是同時結合了 Vue 和 React，在做關於 state 的處理時相當簡潔，原作者也曾寫了另一個叫做 [classcat](https://github.com/JorgeBucaran/classcat) 的專案，大小同樣不大只有 0.3 KB，同樣感受得到極為不易的挑戰性。其實像是 hyperapp 這類型的專案目標不見得是為了要取代某個工具，誠如作者在 README 中所說的，比較像是一種試圖達成某個最小可及目標的嘗試，因為標的明確所以程式碼顯得更為簡短有力且不拖泥帶水。雖然以筆者這樣還很菜的身份講這種話有點ㄎㄅ，但曾經聽業界某位前輩說，整個職業生涯很會用別人家的框架而且用的很順手並不代表你就是一個開發者，更明確的說你可能只是一個對自己會的工具非常擅長的工匠，不是要刻意批評工匠本身，而是在 20 多歲還在衝刺的階段，不要把別人給的東西視作理所當然，有方向性的重造輪子往往會帶來更意想不到的成果。

---

#### Technical Posts - 你都去哪看技術文啊城武

- [ThoughtWorks洞见](http://insights.thoughtworks.cn/)
  
  > 位於中國一個相當具有規模的平台，對於 open source 這塊可以看到不少著墨，之前也有人在[知乎](https://www.zhihu.com/question/24738030)上問過在 ThoughtWorks 工作的感想等等。這個部落格經營蠻長一段時間的了，分類目錄的幾篇文章通讀下來都蠻有感覺的，不過筆者認為其中最讚的是[技術雷達](http://insights.thoughtworks.cn/tech-radar/)，每年 ThoughtWorks 都會固定出兩期，會對於現行市場的各種技術工具諸如框架趨勢及操作細節做出一份具體而微並且長約 20 多頁左右的的 PDF 報告書，這部分在台灣就比較少看到有人在做類似的整理，不過缺什麼就補什麼，台灣同樣有著許多中國不曾存在過的美好和特質，能夠藉由技術社群的力量讓彼此都有所成長再好不過了。

---

#### You Need Some Music, And A Bottle of Dry Martini - 你一定要把氣氛搞得這麼銷魂嗎
- [Porno Graffitti - Anima Rossa](https://www.youtube.com/watch?v=BZckH2RzpTA&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op&index=13)
  
  > 成軍已有 20 多年的實力派樂團，主唱的音色清亮辨識度極高，咬字清晰的特點在唱快歌時發揮尤其明顯。第一次認識色情塗鴉是從死神 Bleach 的這首 opening 聽到的，老實說團名設定真的超奇妙的，從一開始的數位團員相繼因為理念不合離團出走，直到現在留下的兩位包含 vocal 和吉他手都已經是四十多歲的大叔了，雖然是大叔的年紀但只要看過他們現場的演出絕對還是會很嗨，筆者最近也一直在想不曉得到了那樣的年齡，可能 30 歲是一個分水嶺，之後的人生是否仍然對所熱愛的人事物有著同樣的衝勁和執著呢？
  <p align="center"> 
    <a href="https://www.youtube.com/watch?v=BZckH2RzpTA&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op&index=13">
      <img src="https://i.imgur.com/DpOy27t.png" alt="Video Demo" />
    </a>
  </p>


---
> [關於作者](https://goo.gl/1pnqEk)

> [回到首頁](https://git.io/v5wk4)
