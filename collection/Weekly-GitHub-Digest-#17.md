## Weekly-GitHub-Digest #17
> 2017/12/21 - 2017/12/27

#### Web - 網路本身高風險，請詳閱公開說明書
- [tipsy/github-profile-summary](https://github.com/tipsy/github-profile-summary)  Tool for visualizing GitHub profiles
  
  > GitHub 平台的出現改變了整個生態圈，包含對於社群的大力支持投入和擁抱開源文化，本身設計的個人主頁面從一開始的單調到現在的簡約版本都讓筆者非常喜愛，但近期又有開發者針對此一需求推出了更為強大且華麗的版本，還是用 Kotlin 語言進行實作的，我原本一直以為它只能被用來做 Android 相關的用途，沒想到 Web 也開始有應用了。視覺化圖表部分用的是相當主流的 ChartJS，loading spinner 的圖示也蠻療癒的，資料涵蓋 commits 和 stars 數量的整體分析，一年累積下來也方便自我省視。
  <p align="center">
    <a target="_blank" href="https://github.com/tipsy/github-profile-summary"><img alt="github-profile-summary" src="https://i.imgur.com/Jv7r8zb.png"></a>
  </p>
  
- [mxstbr/sharingbuttons.io](https://github.com/mxstbr/sharingbuttons.io)  Quickly generate social sharing buttons with a tiny performance footprint

  > 不管是做網站經營或是一些 side projects 推廣時，總會需要加上幾個社群 icons，方便使用者初來乍到時如果覺得東西不錯便能更方便的被即時分享，以我為例如果是 Web 相關應用的專案，可能會先在 Codepen 做一個簡單的 demo page，然後再加上幾個常用常見的圖示，Facebook，Twitter，VK 等等，在做這塊時其實找了蠻多相關的資源但卻沒一個好用的，偶然挖到的 sharingbuttons 很棒的解決了這個問題，選項亦不過度複雜。
  <p align="center">
    <a target="_blank" href="https://github.com/mxstbr/sharingbuttons.io"><img alt="sharingbuttons.io" src="https://i.imgur.com/72TtdLE.png"></a>
  </p>
---

#### Terminal - 已經是 iTerm 的形狀了呢
- [kpman/newsroom](https://github.com/kpman/newsroom)  💻 A modern CLI to get your favorite news. 📰
  <p align="center">
    <a target="_blank" href="https://github.com/kpman/newsroom"><img alt="newsroom" src="https://i.imgur.com/YuXGsIm.gif"></a>
  </p>
  
  
  > 自從今年三月初開始寫每日文摘之後，都會去幾個常去的站看看是否有新文章，讀過之後覺得有所心得便整理一下，畢竟現在接收的資訊量已經無法用爆炸來形容了，寧願選讀個幾篇文章做為一日總結之後的思考，Chrome 分頁越開越多顯得自己很有效率其實剛好完全相反，寧願多花點時間在幾個相對深入的頁面進行研讀。名字和美劇 The Newsroom 同樣，看過 Will 和 MacKenzie 精彩的對手戲之後也來玩玩看這個方便的工具吧：

  全域安裝：
  ```shell
  $ npm install -g newsroom-cli
  ```
  現在可以使用 `newsroom` 和 `nr` 這兩個指令了，看看 `help` 文件是好習慣：
  ```javascript
  $ newsroom

    Enter an interactive mode to choose your source.

  $ newsroom <source> <number>

    Source:

      Choose one of the following source:
      inside, bnext, nodeweekly, wanqu, techcrunch, codetengu

    Number:

      The amount you want to see at a time. The default is 5.

    Examples:

    - Get wanqu news

      $ newsroom wanqu

    - Get 7 latest TechCrunch news

      $ newsroom techcrunch 7
  ```
  假如說我今天想看灣區日報的最新 5 篇文章：
  ```shell
  $ newsroom wanqu 5
  ```
  如下顯示：
  <p align="center">
    <a target="_blank" href="https://github.com/kpman/newsroom"><img alt="newsroom" src="https://i.imgur.com/RVLhe7T.png"></a>
  </p>
  
  眼尖的開發者應該不難發現 `newsroom` 也用上了筆者前幾期介紹過的 [Inquirer](https://github.com/WeiChiaChang/Weekly-GitHub-Digest/blob/master/collection/Weekly-GitHub-Digest-%2313.md)，像這樣整合各大新聞媒體的服務真的有確實打到痛點。 
  
---

#### Useful OSS - 好用的開源軟體

- [buunguyen/octotree](https://github.com/buunguyen/octotree)  Code tree for GitHub

  > 從命名就看得出該工具的用途了，簡言之就是一個樹狀圖，當你在瀏覽一個開源專案時常會在不同的資料夾之間切換來切換去，有時回到上一層之後又忘記剛剛在哪裡了，在查看中大型專案這種情況尤其頻繁發生，octotree 則是一項簡單安裝在 Chrome 瀏覽器之上便能輕易改善體驗的產品，看了下 Issues 和相關討論串，其實超多人在使用 GitHub 時都有遇上類似的狀況，真正跳出來解決問題的永遠是少數，一方面感謝熱心開發者的時間和心力付出時，另一方面也可以想想自己如何能夠多做多貢獻一點。
  <p align="center">
    <a target="_blank" href="https://github.com/buunguyen/octotree"><img alt="octotree" src="https://i.imgur.com/zrhkfFA.jpg"></a>
  </p>
---

#### Developers - 開發者們

- [Tommy Chen](https://github.com/tommy351)
  
  > 就架設網站這個方面而言 Wordpress 可以說走在相當前面，隨後有 Logdown 以及 Ghost 等等，後來個人網誌的相關需求越趨蓬勃，諸如 Wordpress 這一類的 CMS 極為容易上手，在初期的確很容易調整但到後期卻越來越有種綁手綁腳的感覺，尤其開發者常常只是想找個地方可以專心寫些技術文章而已，並不需要這麼一大包有的沒的 plugin，能夠在平台設定上少點麻煩事少花點不必要的精力總是會讓人生更輕鬆點。Hexo 推出的時間也不短了，時至今日比起一些新潮的框架我還是認為在客製化一些進階調整時依然很順手。以往這塊幾乎都是被像是 Jekyll 和 Octopress 這兩個 blog framework 所瓜分，自從 Hexo 橫空出世後就整個大逆轉，可以看到當年原作者的 [blog 撰文](https://zespia.tw/blog/2012/10/11/hexo-debut/) 留言區還是有不少人回去簽到朝聖。對於許多開發者而言，終其一生都在致力於寫出至少一個具有一定程度影響力的 project，不是追求中，就是正走在追求的道路上。

---

#### Technical Posts - 你都去哪看技術文啊城武

- [Wanqu](https://wanqu.co/b/77/2017-10-30-startup-timeline-reddit.html?s=home)
  
  > 知道灣區日報也是年初的事情，當時覺得可以每天都做閱讀寫作和後續整理很不容易，沒想到三個月後的自己也開始了類似的事情，讀我所讀想我所想，就差加個 bot 讓整個發文流程自動化都完美無缺了。灣區日報每天都會定時推播五篇英文技術相關文章，佐以原作者本身的自我觀點，像個簡單的導讀，但我尤其喜歡這一系列的創業背景故事介紹，過去比較少看到 Reddit 的崛起文，目前看到的幾間大型科技公司和新創原作者都有撰文，對常常做 side projects 的我而言，做產品的心境是接近甚至沒有任何區別的，所以能夠從中汲取點教訓或是經驗都能讓這過程滋潤點。

---

#### You Need Some Music, And A Bottle of Dry Martini - 你一定要把氣氛搞得這麼銷魂嗎
- [SawanoHiroyuki - &Z ft. mizuki](https://www.youtube.com/watch?v=4gMXEd49rbg&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op&index=17)
  
  > 你可能看過在醫龍飾演天才外科醫師坂口憲二的演出，看過多數動漫迷心中的神作 Guilty Crown，也在進擊的巨人中被那充滿無力感的人物眼神所深深震懾住，幾部作品呈現極為不同的劇情和世界觀，唯一的共通點在於背後的音樂選擇和編曲都出自於澤野弘之。總是會有股巨大襲來的滂礡感，動畫 OP 只要配上澤野的樂曲馬上是進入另個完全不同的檔次，瞬間變得熱血無比，但最有意思的在於歌曲命名，非常多奇怪的文字甚至是圖騰都摻雜進來了，多聽幾首之後不難發現歌名常常是混雜著日文英文德文等等，幾個例子如：立body機motion (立體機動)，還有 ətæk 0N tάɪtn (attack on titan 之意)，就像是有貓咪突然跑到鍵盤上亂踩一通所拼湊出來的，後來好像有人發現只要稍微變形轉化一下就可以變成作品中或者其中某位角色的名字，但重點還是在於歌曲本身，不被歌名、歌詞所束縛，也才能自由全心地感受音樂。值得一提的是台灣首次和日本跨國合作的布袋戲電視劇東離劍遊紀，音樂製作也是來自於澤野弘之，雖然他在日本業界可能還不到大師級別，但以他 40 歲不到的年紀對不管是動漫或是日劇迷的眼中已經是神曲製作人一般的存在了。
  <p align="center"> 
    <a href="https://www.youtube.com/watch?v=4gMXEd49rbg&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op&index=17">
      <img src="https://i.imgur.com/TMqAR36.png" alt="Video Demo" />
    </a>
  </p>


---
> [關於作者](https://goo.gl/1pnqEk)

> [回到首頁](https://git.io/v5wk4)
