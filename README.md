# blinnikov
# video advance html
<article role="img" aria-label="cartoon of a person with blue eyes (manga-style)">
  <div class="neck"></div>
  <div class="ear"></div>
  <div class="ear"></div>
  <div class="hair-side"></div>
  <div class="face">
    <div class="mouth"></div>
    <div class="nose"></div>
    <div class="chin"></div>
    <div class="eyebrow"></div>
    <div class="eyebrow"></div>
    <div class="eye"></div>
    <div class="eye"></div>
    <div class="lines"></div>
  </div>
  <div class="bangs bangs-2"></div>
  <div class="bangs bangs-1"></div>
  <div class="bangs bangs-4"></div>
  <div class="bangs bangs-3"></div>
  <div class="bangs bangs-5"></div>
  <div class="bangs bangs-6"></div>
  <div class="bangs bangs-7"></div>
  <div class="bangs bangs-8"></div>
</article>

<a id="youtube" href="https://www.youtube.com/watch?v=kMN-Xd_dcR4" target="_blank">
  <span>See how this demo was coded</span>
</a>
#css
article {
  --skin: #fdb;
  --skin-dark: #eb9;
  --hair: #a86;
  --hair-dark: #975;
  width: 80vmin;
  aspect-ratio: 1;
  overflow: hidden;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  box-shadow: 0 0 0 1vmin;
  background: #ffd;
}

article *,
article *::before,
article *::after {
  position: absolute;
  box-sizing: border-box;
}

.face {
  width: 70%;
  height: 50%;
  background: #00f4;
  top: 10%;
  left: 50%;
  transform: translate(-50%, 0%);
  border-radius:  10% 10% 20% 20% / 100% ;
  background: 
    radial-gradient(450% 80% at 50% -3%, var(--hair) 10.12%, #000 10.25% 11%, var(--skin-dark) 11.125%, #0000 30%),
    var(--skin);
  box-shadow: 
    inset -0.75vmin 0,
    inset 0.75vmin 0,
    inset 3vmin -1vmin 1vmin #0002,
    inset 6vmin -2vmin 2vmin #c002,
    inset -3vmin -1vmin 1vmin #fcc3,
    inset -6vmin -2vmin 2vmin #c662
}

.face::before {
  content: "";
  width: 50%;
  height: 90%;
  top: 60%;
  left: 0.1%;
  background: #0f04;
  border-radius: 0 0 0% 100%;
  transform: skewY(10deg);
  background: 
    radial-gradient(farthest-side at 0 100%, #c002 40%, #0000 80%),
    var(--skin);
/*   border-left: 1vmin solid;
  border-bottom: 0.5vmin solid; */
  clip-path: polygon(0 20%, 100% 20%, 100% 100%, 0 100%);
  box-shadow: 
    inset 0 -0.5vmin,
    inset 0.75vmin 0,
    inset 3vmin 0 1vmin #0002,
    inset 6vmin 0 2vmin #c002,
    inset 0 -3vmin 1vmin -1vmin #c002
}

.face::after {
  content: "";
  width: 50%;
  height: 90%;
  top: 60%;
  right: 0.1%;
  background: #0f04;
  border-radius: 0 0% 100% 0%;
  transform: skewY(-10deg);
  background: 
    radial-gradient(farthest-side at 100% 100%, #c001 40%, #0000 80%),
    var(--skin);
/*   border-right: 0.75vmin solid;
  border-bottom: 0.5vmin solid; */
  clip-path: polygon(0 20%, 100% 20%, 100% 100%, 0 100%);
  box-shadow: 
    inset 0 -0.5vmin,
    inset -0.75vmin 0,
    inset -3vmin 0 1vmin #fcc3,
    inset -6vmin 0 2vmin #c662,
    inset 0 -3vmin 1vmin -1vmin #c002
}

.face * {
  z-index: 1;
}

.mouth {
  width: 14%;
  height: 3%;
  border-radius: 50%;
  border-left: 0.5vmin solid #0000;
  border-top: 0.5vmin solid;
  top: 117%;
  left: 50%;
  transform: rotate(1deg);
  box-shadow: 
    -0.25vmin -0.45vmin 0.2vmin 0.25vmin var(--skin-dark),
    -5.25vmin -0.45vmin 0.2vmin 0.125vmin var(--skin-dark);
}

.mouth::before {
  content: "";
  width: 100%;
  height: 100%;
  border-radius: 0 50% 0 0;
  border-left: 1vmin solid #0000;
  border-top: 0.5vmin solid;
  top: -0.4vmin;
  transform: translate(-90%, 0);
}
.mouth::after {
  content: "";
  width: 50%;
  height: 40%;
  background: #000;
  border-radius: 50% / 0 0 100% 100%;
  top: -0.125vmin;
  transform: translateX(-50%);
}

.nose {
  width: 12%;
  height: 30%;
  top: 70%;
  left: 48%;
}

.nose::after {
  content: "";
  width:100%;
  height: 100%;
  border-radius: 100% / 0 0 45% 20%;
  background: var(--skin);
  box-shadow: 
    inset 0.75vmin -0.5vmin 1.5vmin -0.75vmin #c002,
    inset 1vmin -0.75vmin 2vmin -0.75vmin #fff3;
}

.nose::before {
  content: "";
  width:130%;
  height: 100%;
  border-radius: 100% / 0 0 50% 30%;
  transform-origin: 0 30%;
  transform: rotate(30deg);
  background: linear-gradient(to bottom left, #0000 30%, #c443 0 0);
  filter: blur(0.2vmin);
  box-shadow: 
    -2.5vmin 1.5vmin 1.5vmin -0.75vmin var(--skin-dark),
    -3.5vmin 1.5vmin 2.5vmin -0.5vmin #fff3
}

.lines {
  width: 100%;
  height: 150%;
  background: 
    /*hair*/
    linear-gradient(#000 0 0) 52% 0% / 0.35% 3%,
    linear-gradient(70deg, #0000 45%, #000 0 50%, #0000 0) 51% 1% / 4% 2%,
    linear-gradient(96deg, #0000 45%, #000 0 50%, #0000 0) 53% 1% / 4% 2%,
    /* eyelines */
    radial-gradient(220% 180% at 30% 120%, #0000 50%, #000 51% 52.5%, #0000 53%) 25% 29% / 17% 10%,
    radial-gradient(220% 225% at 60% 120%, #0000 50%, #000 51% 52.25%, #0000 52.5%) 79% 31.25% / 20% 10%,
    linear-gradient(#000 0 0) 30% 46.5% / 1% 0.25%,
    linear-gradient(#000 0 0) 28% 46.65% / 1.5% 0.33%,
    linear-gradient(#000 0 0) 25% 46.65% / 3% 0.33%,
    linear-gradient(#000 0 0) 23% 46.65% / 1% 0.25%,
    
    linear-gradient(#000 0 0) 70% 46.5% / 1% 0.25%,
    linear-gradient(#000 0 0) 72% 46.65% / 1.5% 0.33%,
    linear-gradient(#000 0 0) 75.5% 46.65% / 3% 0.33%,
    linear-gradient(#000 0 0) 77% 46.65% / 1% 0.25%,
    
    /* eyebrow */
    radial-gradient(220% 180% at -40% 120%, #0000 50%, #000 51% 52.5%, #0000 53%) 42% 26.5% / 7% 5%,
    radial-gradient(220% 200% at 140% 120%, #0000 50%, #000 51% 52.5%, #0000 53%) 60% 26.5% / 7% 5%,
    linear-gradient(65deg, #0000 37%, #000 0 45%, #0000 0) 45% 31% / 1% 3%,
    linear-gradient(67deg, #0000 47%, #000 0 50%, #0000 0) 45% 32.5% / 2% 3%,
    
    /* nose */
    linear-gradient(#000 0 0) 47.5% 56.5% / 0.25% 5%,
    linear-gradient(#000 0 0) 47.5% 60% / 0.25% 1%,
    linear-gradient(-45deg, #0000 37%, #000 0 40%, #0000 0) 45.5% 57% / 4% 10%,
    linear-gradient(-45deg, #0000 47%, #000 0 50%, #0000 0) 45% 57.5% / 6% 10%,
    linear-gradient(-47deg, #0000 47%, #000 0 50%, #0000 0) 45% 56.25% / 5% 10%,
    linear-gradient(-47deg, #0000 47%, #000 0 50%, #0000 0) 45.5% 54.5% / 3.5% 10%,
    radial-gradient(150% 120% at 130% -20%, #0000 50%, #000 0 53%, #0000 0) 39% 74% / 12% 13%,
    radial-gradient(150% 120% at -20% 140%, #0000 55%, #000 0 59%, #0000 0) 49% 66% / 7% 7%,
    radial-gradient(150% 100% at 50% 100%, #0000 55%, #000 57% 62.5%, #0000 63%) 55% 69% / 5% 6%,
    /* chin */
    radial-gradient(240% 70% at 70% -5%, #0000 10%, #000 11% 13%, #0000 14%) 44% 100% / 20% 14%,
    radial-gradient(240% 70% at 40% -5%, #0000 20%, #000 21% 33%, #0000 34%) 51% 90% / 12% 4%
/*     ,#f003 */
    ;
  background-repeat: no-repeat;
}

.chin {
  width: 20%;
  height: 6%;
  background: var(--skin-dark);
  border-radius: 50% / 20% 40% 100% 80%;
  top: 127%;
  left: 51%;
  transform: translate(-50%, 0%);
  filter: blur(0.5vmin)
}

.eye {
  background: #fffa;
  width: 25%;
  height: 25%;
  border-radius: 100% / 100% 120% 70% 100%;
  top: 45%;
  left: 13%;
  box-shadow: 
    0.5vmin -1.5vmin 0 -1vmin,
    0 -1vmin 0 -0.5vmin,
    1vmin -2vmin 1vmin -0.5vmin var(--skin-dark),
    -0.5vmin -1vmin 1vmin -0.5vmin #c003,
    -1vmin 1vmin 1vmin -0.5vmin #fff3,
    -0.5vmin 2vmin 1vmin -1.12vmin #c002,
    0 0 0.75vmin #fff
    ;

  overflow: hidden;
}

.eye::before {
  content: "";
  width: 55%;
  height: 110%;
  background:
    radial-gradient(circle at 60% 18%, #fffd 5%, #0000 0),
    radial-gradient(circle at 80% 98%, #fff7 10%, #fff0 35%),
    radial-gradient(at 30% 53%, #fffa 10%, #0000 0),
    radial-gradient(250% 120% at 0 20%, #fffc 20%, #0000 0),
    radial-gradient(#0003 30%, #0000 0),
    linear-gradient(#36aa, #36a8);
  border-radius: 80%;
  top: -10%;
  left: 27%;
  box-shadow: 
    -1vmin 0 0 -0.75vmin,
    1.1vmin 0 0 -0.8vmin;
}

.eye + .eye {
  transform: scaleX(-1);
  left: auto;
  right: 12.5%;
}

.eye + .eye::before {
  transform: scaleX(-1);
}

.eyebrow {
  width: 41%;
  height: 30%;
  border-radius: 100% 200% 50% 0;
  transform: rotate(-7deg);
  top: 36%;
  left: 4%;
  background: linear-gradient(200deg, #c002, #0000 50%);
  box-shadow: 
    1vmin -2.5vmin 0 -1.75vmin,
    inset -1.5vmin 6vmin 1vmin -6vmin var(--skin-dark);
}

.eyebrow + .eyebrow {
  left: auto;
  right: 3.5%;
  width: 40%;
  transform: scaleX(-1) rotate(-8deg);
}


.neck {
  width: 80%;
  height: 30%;
  bottom: 0;
  left: 10%;
}

.neck::before,
.neck::after {
  content: "";
  width: 50%;
  height: 100%;
  border-right: 0.75vmin solid;
  border-bottom: 0.6vmin solid;
  border-radius: 0 0 60% 0;
  transform: scaleX(-1) rotate(-18deg) skew(-3deg);
  
  right: -18%;
  box-shadow:
    3vmin 1vmin 1vmin #fcc3,
    6vmin 2vmin 2vmin #c662,
    0 3vmin 1vmin -1vmin #c002,
    10vmin 10vmin 0 4vmin var(--skin)
}

.neck::after {
  transform: rotate(-20deg) skew(5deg);
  left:-20%;
  box-shadow:
    
    3vmin 1vmin 1vmin #fcc3,
    6vmin 2vmin 2vmin #c662,
    0 3vmin 1vmin -1vmin #c002,
    20vmin 5vmin 2vmin 3vmin var(--skin-dark),
    10vmin 10vmin 0 4vmin var(--skin)
    ;
}

.ear {
  width: 20%;
  height:43%;
  border: 0.75vmin solid;
  border-radius: 60% 120% 70% 120%;
  transform: skewY(-20deg) rotate(-20deg);
  top: 25%;
  left: 10%;
  background: 
    /* lines */
    radial-gradient(130% 150% at 50% 100%, #0000 40%, #000 40.5% 45%, #0000 45.5%) 20% 30% / 30% 30%,
    radial-gradient(130% 250% at 50% 0%, #0000 40%, #000 40.5% 48%, #0000 49%) 37% 49% / 35% 40%,
    linear-gradient(75deg, #0000 45%, #000 0 50%, #0000 0) 20% 85% / 20% 30%,
    /* bg */
    linear-gradient(to right, #0000, var(--skin-dark)),
    linear-gradient(to right, #c002, #0005 ),
    var(--skin);
  background-repeat: no-repeat;
}

.ear::before {
  content: "";
  width: 55%;
  height: 20%;
  border-radius:  50% / 100% 80% 0% 10%;
  border: 0.5vmin solid;
  border-top: 0.75vmin solid;
  left: 12%;
  top: 6%;
  border-bottom: 0;
  background: linear-gradient(#a002, transparent);
}

.ear + .ear {
  background:
    /* lines */
    radial-gradient(130% 150% at 50% 100%, #0000 40%, #000 40.5% 45%, #0000 45.5%) 20% 30% / 30% 30%,
    radial-gradient(130% 250% at 50% 0%, #0000 40%, #000 40.5% 48%, #0000 49%) 37% 49% / 35% 40%,
    linear-gradient(75deg, #0000 45%, #000 0 50%, #0000 0) 20% 85% / 20% 30%,
    /* bg */
    linear-gradient(to right, #0000, var(--skin-dark)),
    linear-gradient(to right, var(--skin), #c005 ),
    var(--skin);
  background-repeat: no-repeat;
  transform: scaleX(-1) skewY(-20deg) rotate(-18deg);
  left: auto;
  right: 9.75%;
}

.hair-side {
  width: 85%;
  height: 85%;
  border: 0.5vmin solid;
  border-radius: 100% / 80% 90% 120% 120%;
  border-left: 0.75vmin solid;
  top: -25%;
  transform: translateX(-50%);
  left: 50%;
  background: 
    var(--hair);
  box-shadow: 
    inset 2vmin 0 1.5vmin #0002,
    inset -3vmin 0 1vmin #fff1
}

.bangs {
  width: 30%;
  height: 30%;
  border-radius: 0 0 100% 0;
  box-shadow: inset -0.5vmin -0.25vmin;
  background: 
    radial-gradient(100% 170% at -10% 0, #0000 58.75%, #000 59% 60.25%, var(--hair-dark) 60.5%, var(--hair) 78%);
  
}

.bangs-1 {
  top: 4%;
  transform: scaleX(-1) translateX(-90%) rotate(-56deg) scale(0.75);
  left: -8%;
  background: 
    radial-gradient(100% 170% at -10% 0, #0000 58.75%, #000 59% 61.25%, var(--hair-dark) 61.5% 70%, var(--hair) 90%);
  box-shadow: inset -0.6vmin -0.4vmin;
}

.bangs-2 {
  left: -22%;
  top: 5%;
  transform: scaleX(-1) translateX(-90%) rotate(-60deg) scale(1.1);
}

.bangs-3 {
  transform: rotate(-60deg) scale(0.7);
  background: 
    radial-gradient(100% 170% at -10% -10%, #0000 63%, #000 63.5% 64.25%, var(--hair-dark) 65% 75%, var(--hair) 90%);
  left: 60%;
  top: 3%;
}
.bangs-4 {
  transform: rotate(-55deg) scale(0.5);
  background: 
    radial-gradient(100% 140% at -10% -5%, #0000 74%, #000 74% 76%, var(--hair-dark) 76.4%, var(--hair) 95%);
  left: 66%;
  top: 3%;
}

.bangs-5 {
  transform: rotate(-50deg) scale(0.6);
  background: 
     radial-gradient(100% 170% at -10% -10%, #0000 64%, #000 64% 66%, #fff1 66.4%),
    radial-gradient(100% 170% at -10% -10%, #0000 64%, #000 64% 66%, var(--hair) 66.4%);
  left: 77.5%;
  top: -7%;
  clip-path: polygon(0 85%, 100% -20%, 100% 100%, 0 100%);
}

.bangs-6 {
  transform: rotate(-40deg) scale(0.9);
  background: 
    radial-gradient(100% 100% at -10% 40%, #0000 63%, #000 63.5% 64.25%, var(--hair-dark) 65%, var(--hair) 75%);
  left: 47%;
  top: 6.25%;
}

.bangs-7 {
  transform: scaleX(-1) rotate(-40deg) scale(0.7);
  background: 
    radial-gradient(100% 100% at -10% 40%, #0000 63%, #000 63.5% 64.25%, var(--hair-dark) 65%, var(--hair) 75%);
  left: 28%;
  top: 4.5%;
  clip-path: polygon(0 -25%, 100% 20%, 100% 100%, 0 100%);
}

.bangs-8 {
  top: -21%;
  transform: scaleX(-1) translateX(-90%) rotate(-86deg) scale(0.75);
  left: -26%;
  background: 
    radial-gradient(100% 170% at -10% 0, #0000 58.75%, #000 59% 61.25%, var(--hair-dark) 61.5% 70%, var(--hair) 90%);
  box-shadow: inset -0.6vmin -0.4vmin;
}



/***/

#youtube {
  z-index: 2;
  display: block;
  width: 100px;
  height: 70px;
  position: absolute;
  bottom: 20px;
  right: 20px;
  background: red;
  border-radius: 50% / 11%;
  transition: transform 0.5s;
}

#youtube:hover,
#youtube:focus {
  transform: scale(1.1);
}

#youtube::before {
  content: "";
  display: block;
  position: absolute;
  top: 7.5%;
  left: -6%;
  width: 112%;
  height: 85%;
  background: red;
  border-radius: 9% / 50%;
}

#youtube::after {
  content: "";
  display: block;
  position: absolute;
  top: 20px;
  left: 40px;
  width: 45px;
  height: 30px;
  border: 15px solid transparent;
  box-sizing: border-box;
  border-left: 30px solid white;
}

#youtube span {
  font-size: 0;
  position: absolute;
  width: 0;
  height: 0;
  overflow: hidden;
}
