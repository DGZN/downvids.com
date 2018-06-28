<template>
  <div class="home">
    <div class="upper-display">
      <div class="row purple-bg">
        <div id="navMenu">
          <div class="col-md-12 col-sm-12 col-xs-12 logo">
            <span>{{ title }}</span>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="header">
          <h1>YouTube Video Downloader</h1>
          <h2>Download videos from YouTube in MP4, FLV, 3GP, and other formats</h2>
        </div>
      </div>
      <div class="searchForm" style="">
        <form id="downloadForm" class="" method="GET" action="https://qdownloader.net/download">
          <input name="video" class="url-input" type="text" placeholder="Enter the video's link..." value="">
          <div id="downloadBtn">Download</div>
        </form>
      </div>
    </div>
      <div class="main front-main">
        <div id="appInfo">
          <div class="site-selection row">
            <h2>More than 800 Websites Supported</h2>
          </div>
          <div class="logos">
            <a href="https://qdownloader.net/youtube-video-downloader">
              <div class="site col-md-2 col-sm-3 col-xs-4">
              <div class="preview">
                <img src="/static/img/sites/youtube.png">
              </div>
              <span>YouTube</span>
            </div>
            </a>
            <a href="https://qdownloader.net/facebook-video-downloader">
              <div class="site col-md-2 col-sm-3 col-xs-4">
              <div class="preview">
                <img src="/static/img/sites/facebook.png">
              </div>
              <span>Facebook</span>
            </div>
            </a>
            <a href="https://qdownloader.net/instagram-video-downloader-photo-downloader">
              <div class="site col-md-2 col-sm-3 col-xs-4">
              <div class="preview">
                <img src="/static/img/sites/instagram.png">
              </div>
              <span>Instagram</span>
            </div>
            </a>
            <a href="https://qdownloader.net/twitter-video-downloader">
              <div class="site col-md-2 col-sm-3 col-xs-4">
              <div class="preview">
                <img src="/static/img/sites/twitter.png">
              </div>
              <span>Twitter</span>
            </div>
            </a>

              <a href="https://qdownloader.net/vimeo-video-downloader">
              <div class="site col-md-2 col-sm-3 col-xs-4">
              <div class="preview">
                <img src="/static/img/sites/vimeo.png">
              </div>
              <span>Vimeo</span>
            </div>
            </a>
              <a href="https://qdownloader.net/liveleak-video-downloader">
              <div class="site col-md-2 col-sm-3 col-xs-4">
              <div class="preview">
                <img src="/static/img/sites/liveleak.png">
              </div>
              <span>LiveLeak</span>
            </div>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Home',
  data () {
    return {
      title: 'DownVids.com'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
    font-weight: normal;
}
h4 {
    font-weight: bold;
    font-size: 18px;
    color: #b4133e;
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: inline-block;
    margin: 0 10px;
}
a {
    color: #42b983;
}
span {
    font-weight: 600;
    font-size: 26px;
    text-decoration: none!important;
    letter-spacing: .3px;
    color: rgb(38, 159, 213);
}
.pBtn{
    background: #6a2884;
    color: #133eb5 !important;
    text-decoration: none!important;
    font-size: 15px;
    font-weight: 500;
    padding: 15px 15px;
    border-radius: 3px;
    display: block;
    width: 250px;
    margin: 0 auto;
    margin-top: 20px;
}
.pBtn:hover{
    color: white !important;
    text-decoration: none !important;
    background: #153385 !important;
}
.logos a {
  position: relative;
  float: left;
}
@media all and (max-width:500px){
    #downloadBtn{
        position:initial!important;
        margin:-1px auto 0!important;
        width:100%!important
   }
    .searchForm input{
        border-radius:3px 3px 0 0!important
   }
}
.upper-display{
    background:rgb(39, 43, 168)!important
}
.upper-display .header{
    color:#fff;
    text-align:center;
    max-width:1100px;
    margin:0 auto;
    padding:45px 10px
}
.upper-display .header h2{
    font-weight:400;
    font-size:20px
}
.site-selection h2{
    position: relative;
    margin: 0 auto;
    font-size:30px;
    font-weight:400;
    color:#223254e6!important;
    margin-bottom:50px
}
.front-main{
   padding:70px 15px!important;
    max-width:900px;
    margin:0 auto;
    text-align:center
}
.site-selection .site{
    margin-bottom:30px
}
.site-selection .site span{
    text-align:center;
    color:#223254e6!important;
    text-decoration:none!important;
    font-weight:700
}

.preview{
    min-height:100px;
    position:relative;
    margin-bottom:10px
}
#downloadBtn,.preview img{
    position:absolute;
    top:0;
    right:0
}
.preview img{
    width:50px;
    bottom:0;
    left:0;
    margin:auto
}
.searchForm{
    padding:0 15px 50px;
    max-width:700px;
    margin:0 auto
}
.error-mssg{
    text-align:center;
    color:#F44336;
    font-weight:600;
    margin-top:30px;
    background:#fafafa;
    border-radius:2px;
    padding:20px 5px;
    font-size:15px
}
.error-mssg ul{
    list-style:none;
    padding:0;
    margin:0;
}
#downloadForm{
   position:relative
}
.url-input{
   width:100%;
   padding-right:15px;
   height:60px;
   box-shadow:inset 0 3px 0 rgba(0,0,0,.04);
   border-radius:3px;
   border:1px solid #e0e0e0;
   background-color:#fff;
   padding-left:55px;
   color:#474756;
   font-size:17px;
   font-weight:400;
   letter-spacing:-.3px;
   background-image:url(https://pickvideo.net/img/input-icon.svg)!important;
   background-repeat:no-repeat!important;
   background-position:center left 12px!important
}
#downloadBtn{
   background:#3c28c4;
   color:#fff;
   font-weight:700;
   line-height:60px;
   width:150px;
   cursor:pointer;
   text-align:center;
   border-radius:0 3px 3px 0
}
#downloadBtn:hover{
   background:#2e1f96!important
}
.spinner{
   margin:0 auto 20px;
   width:70px;
   height:55px;
   text-align:center;
   font-size:10px
}
.spinner>div{
   background-color:#381446;
   height:100%;
   width:7px;
   display:inline-block;
   animation:sk-stretchdelay 1.2s infinite ease-in-out
}
.spinner .rect2{
   animation-delay:-1.1s
}
.spinner .rect3{
   animation-delay:-1s
}
.spinner .rect4{
   animation-delay:-.9s
}
.spinner .rect5{
   animation-delay:-.8s
}
@keyframes sk-stretchdelay{
   0%,100%,40%{
       transform:scaleY(.4);
       -webkit-transform:scaleY(.4)
   }
   20%{
       transform:scaleY(1);
       -webkit-transform:scaleY(1)
   }
}
#loading-message{
   margin-top:40px;
   display:none;
   padding:0 10px
}
#loading-message .status{
   text-align:center;
   font-size:21px;
   color:#4c4c4c
}
.loader{
   font-size:5px;
   margin:30px auto;
   text-indent:-9999em;
   width:11em;
   height:11em;
   border-radius:50%;
   background:#381446;
   background:linear-gradient(to right,#381446 10%,rgba(2,4,1,0) 42%);
   position:relative;
   animation:load3 1.4s infinite linear;
   transform:translateZ(0)
}
.loader:after,.loader:before{
   content:'';
   position:absolute;
   top:0;
   left:0
}
.loader:before{
   width:50%;
   height:50%;
   background:#381446;
   border-radius:100% 0 0
}
.loader:after{
   background:#fff;
   width:75%;
   height:75%;
   border-radius:50%;
   margin:auto;
   bottom:0;
   right:0
}
@keyframes load3{
   0%{
       transform:rotate(0)
   }
   100%{
       transform:rotate(360deg)
   }
}
.downloadSection{
   text-align:center;
   margin-top:50px;
   margin-bottom:50px;
   padding:0 15px
}
.downloadSection .info{
   padding:0 30px
}
.downloadSection .title{
   margin:0 auto;
   color:#223254e6;
   font-weight:600;
   display:block;
   font-size:19px;
   max-width:600px
}
.downloadSection .largeMargin{
   margin-bottom:50px
}
.downloadSection .smallMargin{
   margin-bottom:20px
}
.downloadSection h1{
   font-size:25px;
   margin-bottom:50px
}
.downloadSection h2{
   text-decoration:underline;
   margin-top:50px
}
.downloadSection h3{
   font-size:21px;
   text-decoration:underline
}
.downloadSection img{
   display:block;
   margin:0 auto 16.75px;
   border:1px solid #c5c5c5;
   width:100%;
   max-width:350px
}
.downloadSection .downloadInstruction{
   max-width:800px;
   margin:0 auto 20px;
   display:block;
   font-size:18px;
   color:#6f6f6f
}
.downloadBtn,.downloadBtn:hover{
   color:#fff!important;
   text-decoration:none!important
}
.downloadBtn{
   background:#6a2884;
   font-weight:700;
   font-size:15px;
   margin-bottom:15px;
   border-radius:3px;
   display:inline-block;
   padding:11px 30px
}
.downloadBtn:hover{
   background:#381446!important
}
.downloadsTable{
   width:100%;
   max-width:700px;
   margin:0 auto 100px;
   border-bottom:solid 1px #dedede
}
.downloadsTable tbody{
   background-color:#fafafa
}
.downloadsTable tbody td{
   border-top:solid 1px #dedede;
   padding:21px 7px;
   font-size:16px
}
.downloadsTable tbody td a{
   background:#6a2884;
   color:#fff;
   text-decoration:none!important;
   font-size:13px;
   font-weight:700;
   padding:10px 15px;
   border-radius:3px
}
.downloadsTable tbody td a:hover{
   background:#381446!important;
   color:#fff!important;
   text-decoration:none!important
}
.downloadsTable .headerRow{
   background:#fff;
   font-size:17px
}
.downloadsTable .headerRow th{
   margin-bottom:10px;
   padding:20px 7px
}
@font-face{
   font-family:'Neutrif Pro';
   font-style:normal;
   font-weight:400;
   src:url(/inc/fonts/neutrif_pro_regular-webfont.woff2) format("woff2"),url(/inc/fonts/neutrif_pro_regular-webfont.woff) format("woff"),url(/inc/fonts/https://brixagency.com/wp-content/uploads/2018/02/neutrif_pro_regular-webfont.svg#NeutrifPro) format("svg")
}
@font-face{
   font-family:'Neutrif Pro';
   font-style:normal;
   font-weight:600;
   src:url(/inc/fonts/neutrif_pro_semi_bold-webfont.woff2) format("woff2"),url(/inc/fonts/neutrif_pro_semi_bold-webfont.woff) format("woff"),url(/inc/fonts/neutrif_pro_semi_bold-webfont.svg#NeutrifPro) format("svg")
}
body{
   margin:0 auto!important;
   font-family:"Neutrif Pro",Sans-serif!important;
   background:#fff;
   font-size:15px!important;
   color:#2f2f2fe6!important
}
#navMenu .logo a,#navMenu .menu ul li a{
   color:#fff!important
}
.row{
   margin:0!important
}
.purple-bg{
  background: rgb(33,33,33,.8) !important;

}
#navMenu{
   display:block;
   overflow:hidden;
   padding:20px 55px;
   margin:0 auto
}
#navMenu .logo{
   margin:0;
   padding:0;
   text-align:center
}
#navMenu .menu,#navMenu .menu ul{
   padding:0;
   margin:0;
   text-align:right
}
#navMenu .logo a{
   font-weight:600;
   font-size:26px;
   text-decoration:none!important;
   letter-spacing:.3px
}
#navMenu .menu ul{
   list-style:none
}
#navMenu .menu ul li{
   display:inline-block;
   padding-left:10px;
   padding-right:10px;
   font-weight:400;
   font-size:16px
}
footer{
   background:#381446;
   padding:10px;
   color:#827f84;
   font-size:12px;
   text-align:center
}

</style>
