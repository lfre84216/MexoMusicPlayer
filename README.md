# MexoMusicPlayer
人工智慧語音辨識播放器

## 實作目的
因為自己非常喜歡聽音樂，<br>
從原始的C#開始製作音樂播放器，到後來研究WEB應用程式，<br>
想說是否能夠透過WEB使用語音辨識進行音樂播放，<br>
應而實作研究該專案。

## 設計理念與技術
主要使用WEB應用程式來製作專案，<br>
想要透過語音的方式進行音樂輸入，<br>
同時也可以透過語音的方式進行對音樂進行控制，<br>
在歌曲全數播完後，會有一系列的推薦音樂持續播放。<br>
- MVVM前後端分離
- HTML+CSS
- Flask
- Python-VideosSearch
- Python-pafy
- jQuery+JavaScript
- JSON+Fetch
- KKBOX API
- annyang

## 主要實作功能
實作功能包含完整透過一系列的語音進行音樂播放操作，<br>
同時串接KKBOX API實作出自動推薦播放音樂等功能。<br>
雖然介面顯得有點陽春，但實際的功能都有。
- 語音辨識播放流程 (點播、插播歌曲->說出歌曲名稱->播放音樂)
- 語音辨識音樂控制 (暫停、播放、下一首、切歌、返回初始音量、降低音量、提高音量、調整音量、目前音量)
- 語音對話自動優化播放音量(自動調整音量)
- 自動推薦歌曲播放(KKBOX API)
- 直接下載串流音樂
- 音樂播放速度動態調整

## 相關程式畫面
### Mexo音樂播放<br>
<img src="https://github.com/lfre84216/MexoMusicPlayer/blob/main/1.png">
<br>

### 程式影片DEMO展示
[![IMAGE ALT TEXT HERE](https://github.com/lfre84216/MexoMusicPlayer/blob/main/1.png)](https://www.youtube.com/watch?v=GX6oyUWPhVU)

## 製作過程與困難點
在實作該專案的過程中，<br>
因為對串流音樂非常有興趣，<br>
覺得為什麼音樂不須經過下載，就可以播放出音樂甚至下載，<br>
當初在youtube上面所擁有的歌曲，透過私人伺服器進行快取播放，<br>
即可持續串流該音樂播放一段時間，這也是實作的原理之一。<br><br>
同時透過OAuth2的協定進行驗證，串接了KKBOX的JSON Data API，<br>
也算是學會了資料的API串接功能。<br>
