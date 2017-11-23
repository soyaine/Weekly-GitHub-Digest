## Weekly-GitHub-Digest #12
> 2017/11/16 - 2017/11/22

#### Web - 網路本身高風險，請詳閱公開說明書
- [davidsonfellipe/im-coder](https://github.com/davidsonfellipe/im-coder)  🤘 :trollface:
  
  > 身邊越來越多朋友開始學起寫程式，有時候被問到對於學習這個領域有沒有什麼建議都覺得抖抖的，一方面怕的是稍微不留神一個不小心把這巨大的泡泡戳破，另一方面也擔心亂推人入坑會遭天譴，不過有沒有可以在朋友面前裝裝樣子的開發工具呢？當你提出這個需求的時候茫茫之中勢必會有人真的做出滿足需求的東西，阿扁說過有夢最美希望香水，im-coder 則是讓你美夢成真一鍵成為大神的好物，官方目前釋出了多種熱門語言諸如 JavaScript，Ruby，Python，C 和 Java 等等，雖然大概猜想得到有天才小釣手會跳出來質疑 HTML 到底是不是程式這回事，這個就不在本期週報的討論範疇啦掰哺。
  <p align="center">
    <a target="_blank" href="https://github.com/davidsonfellipe/im-coder"><img alt="im-coder" src="https://i.imgur.com/wPkbOsc.png"></a>
  </p>
  
- [winkerVSbecks/a-triangle-everyday](https://github.com/winkerVSbecks/a-triangle-everyday)  ▲ A triangle everyday for 30 days
  > 幾年前的專案筆者卻是這一兩天才發現，但就算是現在看來仍然有足夠的趣味性存在。日常生活中會出現的物體我們很容易憑藉著直覺說出那是什麼什麼東西，而形狀部分其實並不是那麼被人在意，至少在思考的角度上絕對不會是 priority，圓形正方形長方形明明充斥你我其中卻總是少了點更自然更具體的感受，這個專案的作者很有毅力的製作了連續三十天的三角形，就像是自主性參加 30 天鐵人賽一樣，各種只要聯想得到三角形的概念都可以在這裡頭看到，3D，微互動，SVG 等等，當中個人最為喜愛 [glossy-triangle](https://winkervsbecks.github.io/a-triangle-everyday/glossy-triangle/)，看似普普通通卻能發想出如此多面向的創作，三角形簡單也不簡單，和生活是同樣的。
  <p align="center">
    <a target="_blank" href="https://github.com/winkerVSbecks/a-triangle-everyday"><img alt="a-triangle-everyday" src="https://i.imgur.com/IUIvuO6.png"></a>
  </p>
---

#### Terminal - 已經是 iTerm 的形狀了呢
- [notwaldorf/tiny-care-terminal](https://github.com/notwaldorf/tiny-care-terminal)  💖💻 A little dashboard that tries to take care of you when you're using your terminal
  <p align="center">
    <a target="_blank" href="https://github.com/notwaldorf/tiny-care-terminal"><img alt="tiny-care-terminal" src="https://i.imgur.com/j4h7SGL.png"></a>
  </p>
  
  > 就工作上而言，會從 GUI 的陣營逐漸轉往使用 CLI 並習慣往往是為了讓效率更加提升，而 Terminal 之所以會受到如此多人的愛戴原因實在太多了，~~要感謝的人也太多了，那就謝天吧！~~，如果可以在 CLI 上看到許多即時的資訊顯示，像是高度支援個人配置的 dashboard 一樣的話，使用上應該會更多點樂趣吧：

  簡單的全域安裝：
  ```shell
  $ npm install -g tiny-care-terminal
  ```
  由於 tiny-care-terminal 還加入了 gitstandup 的功能，所以也需要一併安裝：
  ```shell
  $ npm install -g git-standup
  ```
  接著便是設定全域變數，筆者是使用 zshrc 所以做為示範，藉此 tiny-care-terminal 才能撈到資料：
  ```shell
  $ vim ~/.zshrc
  ```
  用 bash 或是 fish 的開發者以此類推，最後可以根據 [sample.env](https://github.com/notwaldorf/tiny-care-terminal/blob/master/sample.env)  給出的範例檔做進階設定：
  ```shell
  export TTC_WEATHER='Taipei'
  export TTC_REPOS='~/Desktop/Side-projects/Code,~/Desktop/Work/Code'
  export TTC_REPOS_DEPTH=2
  export TTC_SAY_BOX='cat'
  ```
  照著 README 之後以下是筆者的 screenshot：
  
  <p align="center">
    <a target="_blank" href="https://github.com/notwaldorf/tiny-care-terminal"><img alt="tiny-care-terminal" src="https://i.imgur.com/s1dIdsn.png"></a>
  </p>
  
  蠻容易上手的，如果有在用 Twitter 的朋友可以再去設定 api key 等參數，最後如果平常有習慣用番茄法做時間管理 tiny-care-terminal 也很貼心的想到了這點：
  
  <p align="center">
    <a target="_blank" href="https://github.com/notwaldorf/tiny-care-terminal"><img alt="tiny-care-terminal" src="https://i.imgur.com/hktYZ2A.png"></a>
  </p>
  
  畫面上的貓咪也可以調整成鳥或是 Mario，真的是把 Ascii arts 發揮的淋漓盡致啊。
  
---

#### Useful OSS - 好用的開源軟體

- [AdiChat/Repository-Hunter](https://github.com/AdiChat/Repository-Hunter)  🌹 Making GitHub:octocat: more socially engaging 🎮 and fun 🍥 for all 

  > GitHub 做為全世界最大的開發者交友平台，其介面向來都非常清爽，不像臉書常常會有置入性廣告，瀏覽起來可能一不小心就過了兩三個小時而忘記原本自己要做的事情了，英文俗諺有句話說：“Fake it until make it.”，聽起來好像沒什麼關聯性也的確是，但 Repository-Hunter 就是試圖要讓 GitHub 看起來更像真的交友網站一樣ＸＤ，感覺有點鬧但功能倒是頗齊全，像是可以查詢自己的相關資訊，還有旁邊 side menu 的部分通常 Popular Users 一欄大概就是某些活躍於特定程式語言領域的大神，然後你就可以看到滿滿的大頭貼了 (◔౪◔)。
  <p align="center">
    <a target="_blank" href="https://github.com/AdiChat/Repository-Hunter"><img alt="Repository-Hunter" src="https://github.com/AdiChat/Repository-Hunter/raw/master/Preview/repository_hunter_1.3.gif"></a>
  </p>
---

#### Developers - 開發者們

- [David Heinemeier Hansson](https://github.com/dhh)
  
  > 寫過 Rails 的應該都對她的老爸 DHH 不陌生，雖然很多人都看衰並靠北 Rails 在做 scale 時的侷限性，誠心建議先捫心自問你家產品真的成長到需要開始擔心這件事了嗎？多的是盲目跟風純粹為了講幹話而講幹話只想製造無謂議題的無聊人士，題外話好像有點扯遠了。長的帥是一回事，程式也寫得好那就真的輸的心服口服了，產品 Basecamp 和 開源框架 Rails 是多數人認識他的代表作，除了開發者的身份之外，他也是位相當專業的賽車手，是曾經拿過比賽冠軍的那種開車程度，筆者撰文至此已經兩眼放空開始質疑起自己的人生。比較好奇的是 Rails 專案已經不在 DHH 個人的 popular repos 了，不曉得是刻意安排的設定亦或是有其他原因就不得而知了。

---

#### Technical Posts - 你都去哪看技術文啊城武

- [Codyhouse](https://codyhouse.co/)  A free library of HTML, CSS, JS nuggets
  
  > Codyhouse 收錄了相當大量的前端應用，偏 widgets 類型的，可以瀏覽到很多以 component 為原型的作品，hero slider，accordion menu 等常見的幾乎都找得到，美中不足的部分可能是 JavaScript 還是以 vanilla 以及 jQuery 為主，在做基於 React 或是 Vue 框架的現代化前端開發可能仍需花點時間調整，同時也要稍微留意一下 license，參考概念並試著用不同的方式實作會比較保險一點。

---

#### You Need Some Music, And A Bottle of Dry Martini - 你一定要把氣氛搞得這麼銷魂嗎
- [Perfume - Sweet Refrain](https://www.youtube.com/watch?v=CYL3DnyA4e0&index=12&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op)
  
  > 和卡莉怪妞同樣是由鬼才製作人中田康貴一手打造的電音團體 Perfume，EDM 曲風一開始聽其實頗不習慣，畢竟原本正常的 vocal 及聲線被刻意壓縮過顯得不太自然，但隔了一陣子會有種必須要再回來重聽幾遍的感覺，接著就是一聽再聽反覆地聽。不過人聲說穿了其實也是音效的一種，很少人會把演唱者的音色本質做大幅度的修改，原因在於過分大膽也過於冒險，中田某種程度打破了這樣的禁忌也成功創造了屬於 Perfume 專屬的 EDM 特質。
  <p align="center"> 
    <a href="https://www.youtube.com/watch?v=CYL3DnyA4e0&index=12&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op">
      <img src="https://i.imgur.com/5Z9gSkI.png" alt="Video Demo" />
    </a>
  </p>


---
> [關於作者](https://goo.gl/1pnqEk)

> [回到首頁](https://git.io/v5wk4)
