## Weekly-GitHub-Digest #11
> 2017/11/09 - 2017/11/15

#### Web - 網路本身高風險，請詳閱公開說明書
- [utatti/pen](https://github.com/utatti/pen)  We need a better Markdown previewer
  
  > 關於寫作又或者是撰寫後端 API 相關文件等事情，最多人也最常用的語法應該非 Markdown 莫屬，而相對應的軟體像是線上版的 [HackMD](https://github.com/hackmdio/hackmd)，線下版有 Macdown 也是許多開發者愛用的工具，至於筆者則是較為喜愛另一款叫做 [Boostnote](https://github.com/BoostIO/Boostnote) 的編輯器，不過這次的重點都不在上述兩者，而是一個更為容易進行寫作的套件，在本機端使用 `npm i -g @noraesae/pen` 全域安裝之後，再打個 `pen TEST.md` 的指令就可以編輯名為 `TEST.md` 的測試文件了，於此同時 server 也一併架起來了，預設 port 會是 6060，編輯器固然好用，但對新工具做點新嘗試也是個不錯的選擇，或許也有其他開發者覺得更習慣更好用也說不定。
  <p align="center">
    <a target="_blank" href="https://github.com/utatti/pen"><img alt="pen" src="https://cloud.githubusercontent.com/assets/1013641/9977359/21b79f66-5f3f-11e5-860a-cf19b2287009.gif"></a>
  </p>
  
- [kevva/brightness](https://github.com/kevva/brightness)  Change screen brightness
  > Mac 調整筆電明暗度已經有 default 按鍵可以直接使用，沒想到竟然還存在著類似這樣功能的神奇 npm module，讓你僅需透過 JavaScript 就可自由控制電腦的明亮程度，雖然亮度範圍的區間目前看來有所侷限，大致上是以 10% 為一個單位。該作者還另外特地打包了一個 [brightness-cli](https://github.com/kevva/brightness-cli)，總感覺這個套件有更多的應用和可能性啊，只是暫時筆者真的想不太到延伸的使用方式。
  <p align="center">
    <a target="_blank" href="https://github.com/kevva/brightness"><img alt="brightness" src="https://i.imgur.com/25PFTGI.png"></a>
  </p>
---

#### Terminal - 已經是 iTerm 的形狀了呢
- [sindresorhus/speed-test](https://github.com/sindresorhus/speed-test)  Test your internet connection speed and ping using speedtest.net from the CLI
  <p align="center">
    <a target="_blank" href="https://github.com/sindresorhus/speed-test"><img alt="speed-test" src="https://i.imgur.com/MYcF1lY.gif"></a>
  </p>
  
  > 這幾天在批踢踢上看到網友分享了[這篇](https://www.ptt.cc/bbs/Gossiping/M.1510488227.A.F6D.html)文章，先不說ＸＸ的壞話啦，重點在測速兩個字，相關工具絕對是琳琅滿目多的數不完，部分學校計算機中心也有提供類似的服務，既然網頁有這樣的應用不意外，然後就很自然的想到了 CLI 有沒有辦法做到類似的效果呢？ 讓 speed-test 測測看吧：

  全域安裝一向是最輕鬆的指令：
  ```shell
  $ npm install --global speed-test
  ```
  接著打開你家的 termianl，看看使用說明：
  ```shell
  $ speed-test --help

  Usage
    $ speed-test

  Options
    -j, --json     Output the result as JSON
    -b, --bytes    Output the result in megabytes per second (MBps)
    -v, --verbose  Output more detailed information
  ```
  嗯嗯，基本上打 `speed-test` 關鍵字就能開始測速了，筆者實測了一下 coworking space 的網速：
  <p align="center">
    <a target="_blank" href="https://github.com/sindresorhus/speed-test"><img alt="speed-test" src="https://i.imgur.com/VtJ15In.png"></a>
  </p>
  看到這樣子的網速表現，腦海中不禁浮現出武哥的那句：世界越快，心則慢。
---

#### Useful OSS - 好用的開源軟體

- [gitshowcase/gitshowcase](https://github.com/gitshowcase/gitshowcase)  Awesome Portfolio from your GitHub

  > 整理履歷從來就不是件容易事，所以 LinkedIn 和 CakeResume 這樣滿足需求的產品才會出現，畢竟十個人的履歷拿來看可能會有十一種完全不同的格式，做軟體的方便之處就是拿個 GitHub 帳號出來看看專案就大概知道平常都在做些什麼，比起面試時扯東扯西說的一口好程式更有說服力。GITSHOWCASE 可以讓你很方便的匯入已登入的 GitHub 帳號和 repos 資料，不管是自己擁有的或是曾經貢獻過的 repos 都可以自由選擇顯示與否，介面上給人一種像是 Bootstrap 混搭 Material 風的感覺，整體而言蠻清爽大方的，如果懶得做高度客製化的個人履歷，短時間又必須生出來的話會是個相對不錯的方式。
  <p align="center">
    <a target="_blank" href="https://github.com/gitshowcase/gitshowcase"><img alt="gitshowcase" src="https://i.imgur.com/BrJGqt2.png"></a>
  </p>
---

#### Developers - 開發者們

- [phodal](https://github.com/phodal)  待我代码编成，娶你为妻可好
  
  > GitHub 雖然主要是個管理程式碼的平台，但也有許多開發者會在上面進行寫作，其實國外蠻多的技術作者常常是先在 GitHub 上寫了不少技術文件之後，接著有書商可能像是 O’Reilly 跑去詢問原作者有無出版意願，筆者沒記錯的話著名的 [You-Dont-Know-JS](https://github.com/getify/You-Dont-Know-JS) 系列就是走這樣的路線。今天要介紹的開發者 phodal 同樣是位多產的技術人兼作家，筆者個人非常喜歡他所撰寫的[我的職業是前端工程師](https://github.com/phodal/fe)，似乎是從村上春樹的《我的職業是一個小說家》那得到啟發的，內容同樣很有意思，值得細讀一番。

---

#### Technical Posts - 你都去哪看技術文啊城武

- [CSS TRICKS](https://css-tricks.com/)
  
  > 目前大概很難找到能夠比 CSS TRICKS 更能把 CSS 相關知識不管是文章或是特定屬性的專題做的如此全面的網站，會有這麼多人推薦不是沒有原因的，但最讓人感動的莫過於他們家的 [License](https://css-tricks.com/license/)，今日的 Web 技術能夠有著這樣蓬勃的發展和生態圈，也總是看得到一群努力的開發者默默的貢獻自己所學並試圖讓整個社群更美好。

---

#### You Need Some Music, And A Bottle of Dry Martini - 你一定要把氣氛搞得這麼銷魂嗎
- [Kenichiro Nishihara - Our love](https://www.youtube.com/watch?v=hYz8GOAMJrQ&index=11&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op)
  
  > 台灣樂壇有著相當豐富的底蘊和文化，鄰國日本同樣存在著許多獨立音樂人和製作者，Kenichiro Nishihara 可以說是其中的佼佼者，擅長以跨界元素讓樂曲組成帶來碰撞刺激和與眾不同的新氣象，爵士的明快節奏和獨到的輕盈感，鋼琴做為背景陪襯再適合不過，也因此聽他的創作很容易不自覺的整個人跟著搖擺了起來。雖然看起來很ㄎㄧㄤ就是了。
  <p align="center"> 
    <a href="https://www.youtube.com/watch?v=hYz8GOAMJrQ&index=11&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op">
      <img src="https://i.imgur.com/VsiHLXe.png" alt="Video Demo" />
    </a>
  </p>


---
> [關於作者](https://goo.gl/1pnqEk)

> [回到首頁](https://git.io/v5wk4)
