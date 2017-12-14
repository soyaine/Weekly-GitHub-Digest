## Weekly-GitHub-Digest #15
> 2017/12/07 - 2017/12/13

#### Web - 網路本身高風險，請詳閱公開說明書
- [szimek/signature_pad](https://github.com/szimek/signature_pad)  HTML5 canvas based smooth signature drawing
  
  > 基於 HTML5 Canvas 一個有趣的小專案，可以讓你在 Web 或是 Mobile 介面都能進行模擬簽名的小工具，支援輸出 PNG 和 SVG 圖檔，有類似需求的情況下挺好用的。發現自己近來關注的東西和以前大不相同，前幾天在看某則關於職場文化的文章時突然想到，從學生到上班族這樣身份上的轉換，其實也意味著更多的未知，可能是單純的憧憬和期待也可能只是個偌大的泡沫，學生時代以為的世界大小其實很有限，吃的可能很省，錢也多數花在升學考試研究所等用途上，但步入職場之後，好像整個世界突然逼著你賺錢，賺得越多才是越成功的，就像是在批踢踢科技版上只要不是在台ＧＧ就會被噓或是年薪沒有至少百萬以上不要叫自己ＲＤ類似的言論層出不窮。變得既複雜又世故，長大難道都是必經的潰爛嗎。
  <p align="center">
    <a target="_blank" href="https://github.com/szimek/signature_pad"><img alt="signature_pad" src="https://i.imgur.com/wkEEKCC.png"></a>
  </p>
  
- [poteto/hiring-without-whiteboards](https://github.com/poteto/hiring-without-whiteboards)  ⭐️ Companies that don't have a broken hiring process

  > 矽谷幾個叫得出名字的大公司採用白板考題面試工程師已經是行之有年的既定事實，但這幾年像是 Rails 它老爸 DHH 在 Twitter 上的[發文](https://twitter.com/dhh/status/834146806594433025?lang=en)和 Mac 必用的 [Homebrew](https://twitter.com/mxcl/status/608682016205344768?lang=en) 作者都跳出來反擊這招募制度，不免讓不少人開始質疑這樣的流程到底能不能夠找到公司最需要的人。暫且不去淌這渾水，至少這個清單列出了目前能夠收集到的所有不採用白板面試的公司，其實還蠻多間的只不過看起來都是英文居多。
  <p align="center">
    <a target="_blank" href="https://github.com/poteto/hiring-without-whiteboards"><img alt="hiring-without-whiteboards" src="https://i.imgur.com/fsjGhZr.png"></a>
  </p>
---

#### Terminal - 已經是 iTerm 的形狀了呢
- [sindresorhus/cli-spinners](https://github.com/sindresorhus/cli-spinners)  Spinners for use in the terminal
  <p align="center">
    <a target="_blank" href="https://github.com/sindresorhus/cli-spinners"><img alt="cli-spinners" src="https://i.imgur.com/KsrUn9L.gif"></a>
  </p>
  
  
  > 在做 CLI 相關應用時常常會有需要跟遠端抓資料的情境出現，既然有抓取的動作那勢必得等東西回傳才有辦法進行下一步的處理，那麼在這期間該怎麼辦呢？總不能就一個空蕩蕩的畫面給使用者看吧，於是便有開發者針對此項需求進行了實作，而其中最多人使用的應該是這套 cli-spinners 了：

  先來安裝一下：
  ```shell
  $ npm install cli-spinners
  ```
  接著在適當的時機時觸發：
  ```javascript
  const cliSpinners = require('cli-spinners');

  console.log(cliSpinners.dots);
  /*
  {
    interval: 80,
    frames: ['⠋', '⠙', '⠹', '⠸', '⠼', '⠴', '⠦', '⠧', '⠇', '⠏']
  }
  */
  ```
  然後你就可以看到一坨點狀的 spinner 開始轉了～
  像這種類似快轉鍵的呈現也有：
  ```javascript
  "arrow3": {
		"interval": 120,
		"frames": [
			"▹▹▹▹▹",
			"▸▹▹▹▹",
			"▹▸▹▹▹",
			"▹▹▸▹▹",
			"▹▹▹▸▹",
			"▹▹▹▹▸"
		]
	}
  ```
  透過簡單更改 `interval` 和 `frames` 這兩項參數即能客製化屬於自己的 spinners。
  除此之外原作也提供了多項不同形狀，詳細可以參考[這份設定](https://github.com/sindresorhus/cli-spinners/blob/master/spinners.json)。
  
---

#### Useful OSS - 好用的開源軟體

- [kmikiy/SpotMenu](https://github.com/kmikiy/SpotMenu)  Spotify in your menu bar

  > 筆者大學時期慣用的筆電是 Windows 系統的，當時為了玩潮潮的 Rails 結果光環境架設就撞了不少牆，不知怎麼搞的最後竟然很果斷的藍屏了... <del>幹什麼東西！ Blue 了！</del>。自從進公司的第一天配了一台亮晶晶的 Mac 之後就回不去了，各種新潮的體驗諸如 iTerm2 的華麗介面和高度個人化配置，聽音樂這部分也開始使用起 Spotify，不過在選擇上一首下一首時並沒有一個較為好用的 dashboard，導致常常要開開關關的有些不方便。SpotMenu 可以透過 `Homebrew` 安裝，操作時會顯示該首單曲的 Thumbnail 和演出者等相關資訊，也有拉條可以改變樂曲的 timeline，不過幾次實測上會出現些小 bug，像是在切換視窗時有時候就突然神隱了，大概十次會有一次類似的情況發生，不過整體而言仍然是個不錯用的軟體。
  <p align="center">
    <a target="_blank" href="https://github.com/kmikiy/SpotMenu"><img alt="SpotMenu" src="https://i.imgur.com/aoiqVF9.gif"></a>
  </p>
---

#### Developers - 開發者們

- [chencheng (云谦)](https://github.com/sorrycc)
  
  > 一位在 alipay 從事前端工程技術研究的開發者，最為人所知的應該非 [dva](https://github.com/dvajs/dva) 莫屬，官方文件同時提供了中英文 README，基於 redux、redux-saga 和 react-router 的一個輕量級前端 framework，很大程度把 Redux 操作上一些不是那麼容易能夠理解的 API 部分簡化，關於 dva 的深入理解可研讀[這篇](https://github.com/dvajs/dva/blob/master/docs/Concepts_zh-CN.md)，但筆者個人會更推薦連同 [knowledgemap](https://github.com/dvajs/dva-knowledgemap) 一同閱讀，幾個核心必懂的語法都囊括了。中國很多技術人都會寫部落格分享，這回當然也不例外的輕易發現了 [blog](https://github.com/sorrycc/blog/issues)，數量約 20 篇左右但可以發現最近猛烈竄起號稱 zero configuration 的 [Parcel](https://github.com/sorrycc/blog/issues/52) 也有一番不錯的討論串。前端就是這樣變化快速，後頭總有人想打造出更屌的工具取代當前的霸主，外頭的人看來就是無數次的重造輪子自討苦吃，但真的是這樣嗎？有很大的原因是<b>當前的輪子雖然可以用但 still not good enough</b>，總有些概念是在每次更迭中極少改變過的。Elon Musk 所說的[第一性原理](https://softnshare.wordpress.com/2017/04/29/elonmuskfirstprinciple/)筆者是高度認同的，做為開發者應該花時間投入並專注的層面在於撇開事物表象，發現其核心本質，然後一步一步往上走。

---

#### Technical Posts - 你都去哪看技術文啊城武

- [GitHub for Open Source / Community Stories](https://github.com/open-source/stories)
  
  > GitHub 在一般印象中最常被使用的功能除了上傳程式以外，像 Community 等其他 features 或是資源就不是這麼多人知道了，其實 GitHub 在 [open source](https://github.com/open-source) 這圈子已耕耘多年，透過這些資料或多或少能讓自己更為熟悉開源文化的美好之處。雖然嚴格來說這不能算是技術相關的部落格，但廣義上而言也是一種質量兼具的分享形式，這是 GitHub 專門收集各種開源框架和工具背後故事的一個網站，最早是先看到 Vue 的作者 Evan You 在上面的 [story](https://github.com/open-source/stories/yyx990803)，後來又挖到了像是 Babel 目前的主要維護[開發者](https://github.com/open-source/stories/hzoo)等等，英文用字相當淺顯易懂，內容也比想像中的要有趣多了，筆者真心力推。

---

#### You Need Some Music, And A Bottle of Dry Martini - 你一定要把氣氛搞得這麼銷魂嗎
- [Joe hisaishi - hope and legacy](https://www.youtube.com/watch?v=hLrbkl__x5s&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op&index=15)
  
  > 儘管已在多部動畫電影久聞日本大師級人物久石讓的樂曲創作，但身為一個不專業的粉絲首次關注到 Hope And Legacy 一曲卻是在[羽生結弦](https://www.youtube.com/watch?v=yZxDCfgVfTc)於今年四月的花滑世錦賽才聽到，行雲流水的明快節奏，每一回跳躍既動感亦自然。既然都談到羽生結弦了，不妨再把內容深入一點。不管在中國日本亦或是花滑大國俄羅斯都擁有著極高人氣，比賽結束之後總是在謝幕時會下起著名的維尼熊雨，數量多到要用那種黑色超大的塑膠袋才裝得完，誇張程度可能唯有親臨現場支持才有辦法感受了。和筆者同樣是 23 歲的年紀，卻已多次打破世界紀錄，一次又一次的表演都期待著他將帶來怎樣的突破和驚喜，就如同多項運動一樣，羽生結弦所立下的多道障礙包括短曲和長曲項目等等，除非有另個花滑界超新星的出現，這紀錄大概只有他本人能破了，至少在這個世紀看來可能是這樣。
  <p align="center"> 
    <a href="https://www.youtube.com/watch?v=hLrbkl__x5s&list=PLxPPbs7D6-e9EormZGytI5kUtNiOre2Op&index=15">
      <img src="https://i.imgur.com/LVBrKAY.png" alt="Video Demo" />
    </a>
  </p>


---
> [關於作者](https://goo.gl/1pnqEk)

> [回到首頁](https://git.io/v5wk4)
