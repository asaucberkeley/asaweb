---
title: ASA @ Cal
layout: home
description: Jekyll Serif contains content types for a typical business website. The theme is fully responsive, blazing fast and artfully illustrated.
intro_image: "images/logo/asalanding.png"
intro_image_absolute: true
intro_image_hide_on_mobile: true
show_call_box: true
---

# Afghan Student Association

Welcome to UC Berkeley’s Afghan Student Association, a place to learn about the culture, heritage, and traditions of Afghan peoples.

 با درود! به انجمن دانشجویان افغان برکلی خوش آمدید؛ جایی برای آشنایی با فرهنگ، سنت ها و آداب و رسوم مردم افغانستان 
 
  سلامونه! د يوسي برکلې د افغان سټوډنټ ټولنې ته ښه راغلاست، د افغانانو د کلتور، ميراث او دودونو په اړه د زده کړې ځاې

<!-- Support of Iran button -->
<link href="https://assets.calendly.com/assets/external/widget.css" rel="stylesheet">
<script src="https://assets.calendly.com/assets/external/widget.js" type="text/javascript" async></script>
<script type="text/javascript">window.onload = function() { Calendly.initBadgeWidget({ url: 'images/iranstatement.pdf', text: 'ASA offical statement supporting Iranians', color: '#E5261F', textColor: '#ffffff', branding: undefined }); }</script>
<!-- end -->

<!-- -->
<link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
    <!--Stylesheets-->
    <style media="screen">
      *,
*:before,
*:after{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}
body{
    background-color: #0855ae;
}
.popup{
    background-color: #ffffff;
    width: 420px;
    padding: 30px 40px;
    position: absolute;
    transform: translate(-50%,-50%);
    left: 50%;
    top: 50%;
    border-radius: 8px;
    font-family: "Poppins",sans-serif;
    display: none; 
    text-align: center;
}
.popup button{
    display: block;
    margin:  0 0 20px auto;
    background-color: transparent;
    font-size: 30px;
    color: #ffffff;
    background: #03549a;
    border-radius: 100%;
    width: 40px;
    height: 40px;
    border: none;
    outline: none;
    cursor: pointer;
}
.popup h2{
  margin-top: -20px;
}
.popup p{
    font-size: 14px;
    text-align: justify;
    margin: 20px 0;
    line-height: 25px;
}
a{
    display: block;
    width: 150px;
    position: relative;
    margin: 10px auto;
    text-align: center;
    background-color: #0f72e5;
    border-radius: 20px;
    color: #ffffff;
    text-decoration: none;
    padding: 8px 0;
}
    </style>
</head>
<body>
    <div class="popup">
        <button id="close">&times;</button>
        <h2>Automatic Pop-Up</h2>
        <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Expedita distinctio fugiat alias iure qui, commodi minima magni ullam aliquam dignissimos?
        </p>
        <a href="#">Let's Go</a>
    </div>
    <!--Script-->
    <script type="text/javascript">
window.addEventListener("load", function(){
    setTimeout(
        function open(event){
            document.querySelector(".popup").style.display = "block";
        },
        2000 
    )
});


document.querySelector("#close").addEventListener("click", function(){
    document.querySelector(".popup").style.display = "none";
});
    </script>
