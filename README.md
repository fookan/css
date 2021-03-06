@charset "UTF-8";
/*/////////////////////////////////////////////////
//twitter風チャット画面(会話方式)を記事に表示する方法
/////////////////////////////////////////////////*/
.twitter__container {
  padding: 0;
  background: #ffffff;
  overflow: hidden;
  max-width: 400px;
  margin: 20px auto;
  font-size: 80%;
  border: solid 1px #eeeeee;
}

.twitter__container a {
  color: #58aeed;
}

/* タイトル部分 */
.twitter__container .twitter__title {
  background: #58aeed;
  padding: 10px;
  text-align: center;
  font-size: 150%;
  color: #ffffff;
}

.twitter__container .twitter__title .twitter-logo {
  margin: 0 auto;
  width: 20px;
  height: 20px;
  display: block;
  background: url(svg/twitter-logo.svg) center no-repeat;
}

.twitter__container .twitter__title span {
  font-size: 20px;
}

/* タイムライン部分 */
.twitter__container .twitter__contents {
  overflow: hidden;
  position: relative;
  line-height: 135%;
}

.twitter__container .twitter__contents.scroll {
  height: 500px;
  overflow-y: scroll;
}

.twitter__container .twitter__block {
  width: 100%;
  display: block;
  padding: 10px;
  margin-bottom: 5px;
  border-bottom: solid 1px #eeeeee;
  overflow: hidden;
}

.twitter__container .twitter__block:last-child {
  border-bottom: solid 0px;
}
/* アイコン画像 */
.twitter__container .twitter__block figure {
  width: 50px;
  padding: 0;
  margin: 0;
  float: left;
  width: 50px;
}
  /* 正方形を用意 */
.twitter__container .twitter__block figure img {
  border-radius: 50%;
  width: 50px;
  height: 50px;
}
/* コメントエリア */
.twitter__container .twitter__block-text {
  margin: 0;
  position: relative;
  margin-left: 60px;
  padding-right: 10px;
}

.twitter__container .twitter__block-text .name {
  font-weight: bold;
}

.twitter__container .twitter__block-text .name .name_reply {
  color: #8a9aa4;
  margin-left: 10px;
}

.twitter__container .twitter__block-text .date {
  position: absolute;
  top: 0;
  right: 20px;
  text-align: right;
  color: #8a9aa4;
}
/* 本文 */
.twitter__container .twitter__block-text .text {
  margin: 5px 0;
}
/* 画像を貼る場合 */
.twitter__container .twitter__block-text .text .in-pict img {
  border-radius: 20px;
  -webkit-border-radius: 20px;
  -moz-border-radius: 20px;
  margin: 5px 0;
  width: 95%;
  height: 200px;
  object-fit: cover;
}

/*///////////////////////////////////////////
//埋め込みアイコン
////////////////////////////////////////////*/

.twitter__container .twitter__icon br{
  display: none;
}

.twitter__container .twitter__icon .twitter-bubble {
  width: 14px;
  height: 14px;
  display: block;
  padding-left: 20px;
  background: url("svg/twitter-bubble.svg") left no-repeat;
  width: 20%;
  float: left;
  color: #8a9aa4;
}

.twitter__container .twitter__icon .twitter-heart {
  width: 14px;
  height: 14px;
  display: block;
  padding-left: 20px;
  background: url("svg/twitter-heart.svg") left no-repeat;
  width: 20%;
  float: left;
  color: #8a9aa4;
}

.twitter__container .twitter__icon .twitter-loop {
  width: 14px;
  height: 14px;
  display: block;
  padding-left: 20px;
  background: url("svg/twitter-loop.svg") left no-repeat;
  width: 20%;
  float: left;
  color: #8a9aa4;
}


<html lang="ja">
<head>
  <meta charset="UTF-8"/>
  <title>twitter風チャット画面(会話方式)を記事に表示する方法 │ ナコさんのブログ nako-log WEB小ネタと生活ライフハック</title>
  <link rel='stylesheet' href='style.css' type='text/css' media='all' />
</head>
<body>

  <!-- ▼twitter風ここから -->
  <div class="twitter__container">
    <!-- タイトル -->
    <div class="twitter__title">
      <span class="twitter-logo"></span>
    </div>

    <!-- ▼タイムラインエリア scrollを外すと高さ固定解除 -->
    <div class="twitter__contents scroll">

      <!-- 記事エリア -->
      <div class="twitter__block">
        <figure>
          <img src="icon.png" />
        </figure>
        <div class="twitter__block-text">
          <div class="name">うさきち<span class="name_reply">@usa_tan</span></div>
          <div class="date">10分前</div>
          <div class="text">
            今日も終電だよ～<br>
          </div>
          <div class="twitter__icon">
            <span class="twitter-bubble"></span>
            <span class="twitter-loop"></span>
            <span class="twitter-heart"></span>
          </div>
        </div>
      </div>

      <!-- 記事エリア -->
      <div class="twitter__block">
        <figure>
          <img src="icon.png" />
        </figure>
        <div class="twitter__block-text">
          <div class="name">うさきち<span class="name_reply">@usa_tan</span></div>
          <div class="date">1時間前</div>
          <div class="text">
            残業でお腹空いたから朝までやってるお店でラーメン食べることにした(^o^)神の食べ物すぎる・・うまぁ
            <div class="in-pict">
              <img src="sample.jpg">
            </div>
          </div>
          <div class="twitter__icon">
            <span class="twitter-bubble">1</span>
            <span class="twitter-loop">4</span>
            <span class="twitter-heart">122</span>
          </div>
        </div>
      </div>

      <!-- 記事エリア -->
      <div class="twitter__block">
        <figure>
          <img src="icon.png" />
        </figure>
        <div class="twitter__block-text">
          <div class="name">うさきち<span class="name_reply">@usa_tan</span></div>
          <div class="date">2018/06/24 5:34</div>
          <div class="text">
            睡眠２時間で出社なんだけど…
            <a href="https://nakox.jp/">https://nakox.jp/</a>
          </div>
          <div class="twitter__icon">
            <span class="twitter-bubble">1</span>
            <span class="twitter-loop"></span>
            <span class="twitter-heart"></span>
          </div>
        </div>
      </div>


    </div>
    <!--　▲タイムラインエリア ここまで -->
  </div>
  <!--　▲twitter風ここまで -->

</body>

</html>

// SVG
// twitter-heart.svg
```
<?xml version="1.0" encoding="utf-8"?>
<!-- Generator: Adobe Illustrator 22.1.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
<svg version="1.1" id="レイヤー_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px"
	 y="0px" viewBox="0 0 512 512" style="enable-background:new 0 0 512 512;" xml:space="preserve">
<style type="text/css">
	.st0{fill:#8A9AA4;}
</style>
<title></title>
<g id="icomoon-ignore">
</g>
<path class="st0" d="M377.6,32c-53.8,0-100.1,43.8-121.6,89.5C234.5,75.8,188.2,32,134.4,32C60.2,32,0,92.2,0,166.4
	c0,150.9,152.2,190.5,256,339.7c98.1-148.3,256-193.6,256-339.7C512,92.2,451.8,32,377.6,32L377.6,32z"/>
</svg>
```

twitter-loop
```

<?xml version="1.0" encoding="utf-8"?>
<!-- Generator: Adobe Illustrator 22.1.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
<svg version="1.1" id="レイヤー_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px"
	 y="0px" viewBox="0 0 512 512" style="enable-background:new 0 0 512 512;" xml:space="preserve">
<style type="text/css">
	.st0{fill:#8A9AA4;}
</style>
<title></title>
<g id="icomoon-ignore">
</g>
<path class="st0" d="M64,160h320v96l128-128L384,0v96H0v192h64V160z M448,352H128v-96L0,384l128,128v-96h384V224h-64V352z"/>
</svg>
```

twitter-bubble
```

<?xml version="1.0" encoding="utf-8"?>
<!-- Generator: Adobe Illustrator 22.1.0, SVG Export Plug-In . SVG Version: 6.00 Build 0)  -->
<svg version="1.1" id="レイヤー_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px"
	 y="0px" viewBox="0 0 512 512" style="enable-background:new 0 0 512 512;" xml:space="preserve">
<style type="text/css">
	.st0{fill:#8A9AA4;}
</style>
<title></title>
<g id="icomoon-ignore">
</g>
<path class="st0" d="M256,32c141.4,0,256,93.1,256,208S397.4,448,256,448c-13.6,0-26.9-0.9-39.9-2.5c-55,55-120.6,64.9-184.1,66.3
	v-13.5c34.3-16.8,64-47.4,64-82.3c0-4.9-0.4-9.7-1.1-14.3C37,363.5,0,305.3,0,240C0,125.1,114.6,32,256,32L256,32z"/>
</svg>
```
