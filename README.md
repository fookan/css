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
