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
<h1>
  <a href="" class="typewrite" data-period="2000" data-type='[ "با درود", "سلامونه", "welcome", "خوش آمدید" ]'>
    <span class="wrap"></span>
  </a>
</h1>
<style>
    body {
  background-color:#fff;
  text-align: center;
  color:black;
  padding-top:10em;
}

* { color:black; text-decoration: none;}
</style>
<script>
    var TxtType = function(el, toRotate, period) {
        this.toRotate = toRotate;
        this.el = el;
        this.loopNum = 0;
        this.period = parseInt(period, 10) || 2000;
        this.txt = '';
        this.tick();
        this.isDeleting = false;
    };

    TxtType.prototype.tick = function() {
        var i = this.loopNum % this.toRotate.length;
        var fullTxt = this.toRotate[i];

        if (this.isDeleting) {
        this.txt = fullTxt.substring(0, this.txt.length - 1);
        } else {
        this.txt = fullTxt.substring(0, this.txt.length + 1);
        }

        this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

        var that = this;
        var delta = 200 - Math.random() * 100;

        if (this.isDeleting) { delta /= 2; }

        if (!this.isDeleting && this.txt === fullTxt) {
        delta = this.period;
        this.isDeleting = true;
        } else if (this.isDeleting && this.txt === '') {
        this.isDeleting = false;
        this.loopNum++;
        delta = 500;
        }

        setTimeout(function() {
        that.tick();
        }, delta);
    };

    window.onload = function() {
        var elements = document.getElementsByClassName('typewrite');
        for (var i=0; i<elements.length; i++) {
            var toRotate = elements[i].getAttribute('data-type');
            var period = elements[i].getAttribute('data-period');
            if (toRotate) {
              new TxtType(elements[i], JSON.parse(toRotate), period);
            }
        }
        // INJECT CSS
        var css = document.createElement("style");
        css.type = "text/css";
        css.innerHTML = ".typewrite > .wrap { border-right: 0.08em solid #fff}";
        document.body.appendChild(css);
    };
</script>

<!-- Anti Shiite Stement button -->
<link href="https://assets.calendly.com/assets/external/widget.css" rel="stylesheet">
<script src="https://assets.calendly.com/assets/external/widget.js" type="text/javascript" async></script>
<script type="text/javascript">window.onload = function() { Calendly.initBadgeWidget({ url: 'images/antiahiastatement.pdf', text: 'ASA offical statement against Anti-Shiite Behavior', color: '#E5261F', textColor: '#ffffff', branding: undefined }); }</script>
<!-- end -->
<br/>
<!-- Support of Iran button -->
<link href="https://assets.calendly.com/assets/external/widget.css" rel="stylesheet">
<script src="https://assets.calendly.com/assets/external/widget.js" type="text/javascript" async></script>
<script type="text/javascript">window.onload = function() { Calendly.initBadgeWidget({ url: 'images/iranstatement.pdf', text: 'ASA offical statement supporting Iranians', color: '#E5261F', textColor: '#ffffff', branding: undefined }); }</script>
<!-- end -->
