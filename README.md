# site1.css

* {
margin: 0;
padding: 0;
box-sizing: border-box;
}

.imagem-cabecares, .imagem-unitingres, .imagem-rodares{
visibility: hidden;
}

.quadrado-hamburguer{
background-color: #2f2c2f;
width:40px;
height:39px;
position:absolute;
left:0px;
top:10px;
visibility: hidden;
}

.top-nav {
display: flex;
flex-direction: row;
align-items: center;
justify-content: space-between;
/* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
color: rgb(202, 0, 0);
height: 50px;
padding: 1em;
}

.menu-hamburguer {
display: flex;
flex-direction: row;
list-style-type: none;
margin: 0;
padding: 0;
visibility: hidden;

}

.menu-hamburguer > .li {
margin: 0 1rem;
overflow: hidden;

}

.menu-button-container {
display: none;
height: 10%;
width: 10px;
cursor: pointer;
flex-direction: column;
justify-content: center;
align-items: center;
position:absolute;
left:217px;
top:-4px;
z-index: 9999;

}

#menu-toggle {
display: none;

}


.menu-button,
.menu-button::before,
.menu-button::after {
display: block;
background-color:  #ff4e5b;
position: absolute;
height:3px;
width: 22px;
transition: transform 400ms cubic-bezier(0.23, 1, 0.32, 1);
border-radius: 2px;

}

.menu-button::before {
content: '';
margin-top: -7px;
}

.menu-button::after {
content: '';
margin-top: 7px;

}

#menu-toggle:checked + .menu-button-container .menu-button::before {
margin-top: 0px;
transform: rotate(405deg);

}

#menu-toggle:checked + .menu-button-container .menu-button {
background: rgba(255, 255, 255, 0);
}

#menu-toggle:checked + .menu-button-container .menu-button::after {
margin-top: 0px;
transform: rotate(-405deg);
}

.logo2{
visibility: hidden;
}

@media (max-width: 700px){
.menu-button-container {
display: flex;
}
}


.menu-hamburguer {
position: absolute;
top: 0;
margin-top: 50px;
left: 0;
flex-direction: column;
width: 100%;
justify-content: center;
align-items: center;
visibility: visible;
z-index: 999;
position: absolute;
top:120px;
z-index: 9999;
}



#menu-toggle ~ .menu-hamburguer  .li {
height: 0;
margin: 0;
padding: 0;
border: 0;
transition: height 400ms cubic-bezier(0.23, 1, 0.32, 1);
z-index: 9999;
}



#menu-toggle:checked ~ .menu-hamburguer  .li {
border: 1px solid #333;
height: 2.5em;
padding: 0.5em;
transition: height 400ms cubic-bezier(0.23, 1, 0.32, 1);
z-index: 9999;
}


.menu-hamburguer  > .li {
display: flex;
justify-content: center;
margin: 0;
padding: 0.5em 0;
width: 100%;
color: white;
background-color: #222;
z-index: 9999;
}



.menu-hamburguer  > li:not(:last-child) {
border-bottom: 1px solid #444;
}


.quadrado-hamburguer{
visibility: hidden;
z-index: 999;
}



.imagem-cabeca{
width: 100%;
height:741px;
position:absolute;
left:0px;
top:0px;
}

.retangulo-foto{
width:100%;
height:85px;
background-color: #ffffff;
position:absolute;
left:0px;
top:741px;
z-index: 999;
}

.menu {
display: flex;
justify-content: center;
align-items: center;
width: 95%;
margin: 0 auto;
font-family: arial, helvetica, sans-serif;
font-size: 16px;
font-weight: 400;
font-style: normal;
color: #ffffff;
text-decoration: none;
border-color: transparent;
position:absolute;
left:-291px;
top:2px;
}

#about{
position:relative;
right:4px;
}

#pages{
position:relative;
left:4.8px;
}

.seta{
width:10px;
height:11px;
margin-left:8px;
position: relative;
top:1px;
}

#blog{
position:relative;
left:2.3px;
}

#gallery{
position:relative;
right:3.3px;
}

#contacts{
position:relative;
left:5.5px;
}


ol {
display: flex;
flex-wrap: wrap;
align-items: center;
justify-content: center;
width: 100%;
margin: 0 auto;
padding: .5em 0;
list-style: none; 
}

#drop{
background: #444;
width:180px;
}

.menu-item {
/*  */
padding: 1em .4em;
position: relative;
border-bottom: 2px solid transparent ;
margin: 0 .0.8em;
transition: border-bottom .23s ease-in-out, background .23s linear;
cursor: pointer;
min-width: 5.9em;
text-align: center;
width:20px;

}

/* .menu-item[aria-haspopup="true"] {
border-bottom-color: #fc9b1b;
} */

.menu-item:hover, .menu-item:focus-within {
border-bottom-color: #91d36b;
width:10px;
/* background: #333;  */
}

.menu-item:hover .sub-menu, .menu-item:hover .sub-menu:hover, .menu-item:focus-within .sub-menu, .menu-item:focus-within .sub-menu:hover {
visibility: visible;
opacity: 1;
display: flex; 
}

.sub-menu {
flex-direction: column;
align-items: flex-start;
position: absolute;
left: 0;
margin-top: 1.3em;
visibility: hidden;
display: none;
opacity: 0;
}

.sub-menu .menu-item {
margin: .1em 0;
padding: 1em;
width: 13em;
text-align: center;
z-index: 2; 
}

a {
color: #fff;
text-decoration: none;
/* text-transform: uppercase;  */
}

a:focus {
outline: none; 
}

.icon-busca{
position:absolute;
left:1338px;
top:28px;
width:19px;
height:19px;
}

.titulo1{
font-weight: 400;
font-style: normal;
font-family: 'Pacifico', handwriting;
color: #ff4e5b;
font-size: 36px;
line-height: 1;
letter-spacing: 0px;
position:absolute;
left:188px;
top:162px;
z-index: 9999;
}

.titulo2{
font-weight: 400;
font-style: normal;
font-family: 'Pacifico', handwriting;
color: #ffffff;
font-size: 36px;
line-height: 1;
letter-spacing: 0px;
position:absolute;
left:292.4px;
top:162px;
}

.texto-titulo{
font-weight: 300;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: rgba(255,255,255,0.4);
font-size: 14px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:188px;
top:218px;
}

.numero-registo{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 30px;
line-height: 1.2;
letter-spacing: 0px;
position:absolute;
left:588px;
top:162px;
z-index: 9999;
}

.texto-register{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 16px;
line-height: 1.7;
letter-spacing: 0px;
position:absolute;
left:588px;
top:198px;
}

.android{
position:absolute;
left:924.5px;
top:162px;
}

.apple{
position:absolute;
left:1137px;
top:162px;
}

.casal-beijando{
position:absolute;
left:492px;
top:328px;
width:865px;
z-index: 999;
}

.titulo-find1{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 60px;
line-height: 1.2;
letter-spacing: 0px;
text-shadow: 5px 5px 15px rgb(0 0 0 / 70%);
position:absolute;
left:188px;
top:388px;
z-index: 9999;
}

.titulo-find2{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 60px;
line-height: 1.2;
letter-spacing: 0px;
text-shadow: 5px 5px 15px rgb(0 0 0 / 70%);
position:absolute;
left:188px;
top:460px;
z-index: 9999;
}

.botao-cabeca{
font-family: 'Ubuntu', sans-serif;
font-weight: 400;
font-style: normal;
color: #f7f7f7;
background-color: #ff4e5b;
border-color: transparent;
border-radius: 90px;
width:210px;
height:60px;
font-size: 18px;
line-height: 24px;
text-align: center;
cursor: pointer;
position:absolute;
left:187px;
top:592px;
}

.imagem-welcome{
position:absolute;
left:187px;
top:914px;
}

.titulo-welcome{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 36px;
line-height: 1.2;
letter-spacing: 0px;
position:absolute;
left:921.3px;
top:914px;
}

.texto-welcome{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 18px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:921.3px;
top:984px;
width:27%;
}

.titulo-sobimagem-tired{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 60px;
line-height: 1.2;
letter-spacing: 0px;
position:absolute;
left:688px;
top:1233px;
width:45%;
}

.botao-welcome{
font-family: 'Ubuntu', sans-serif;
font-weight: 400;
font-style: normal;
color: #f7f7f7;
background-color: #ff4e5b;
border-color: transparent;
border-radius: 90px;
width:194px;
height:60px;
font-size: 18px;
line-height: 24px;
text-align: center;
cursor: pointer;
position:absolute;
left:920px;
top:1422px;
}

.titulo-last{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 36px;
line-height: 1.2;
letter-spacing: 0px;
position:absolute;
left:603px;
top:1711px;
}

.imagem-profile1{
position:absolute;
left:187px;
top:1815px;
}

.nome-donna{
color: #ff4e5b;
text-decoration: none;
font-weight: 700;
font-style: normal;
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:188px;
top:2000px;
}

.age-dona{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #b6b6b6;
font-size: 14px;
line-height: 2;
letter-spacing: 0px;
position:absolute;
left:188px;
top:2025px;
}

.imagem-profile2{
position:absolute;
left:387px;
top:1815px;
}

.nome-walter{
color: #ff4e5b;
text-decoration: none;
font-weight: 700;
font-style: normal;
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:388px;
top:2000px;
}

.age-walter{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #b6b6b6;
font-size: 14px;
line-height: 2;
letter-spacing: 0px;
position:absolute;
left:388px;
top:2025px;
}


.imagem-profile3{
position:absolute;
left:587px;
top:1815px;
}

.nome-sarah{
color: #ff4e5b;
text-decoration: none;
font-weight: 700;
font-style: normal;
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:588px;
top:2000px;
}

.age-sarah{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #b6b6b6;
font-size: 14px;
line-height: 2;
letter-spacing: 0px;
position:absolute;
left:588px;
top:2025px;
}

.imagem-profile4{
position:absolute;
left:787px;
top:1815px;
}

.nome-danielle{
color: #ff4e5b;
text-decoration: none;
font-weight: 700;
font-style: normal;
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:788px;
top:2000px;
}

.age-danielle{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #b6b6b6;
font-size: 14px;
line-height: 2;
letter-spacing: 0px;
position:absolute;
left:788px;
top:2025px;
}

.imagem-profile5{
position:absolute;
left:987px;
top:1815px;
}

.nome-john{
color: #ff4e5b;
text-decoration: none;
font-weight: 700;
font-style: normal;
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:988px;
top:2000px;
}

.age-john{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #b6b6b6;
font-size: 14px;
line-height: 2;
letter-spacing: 0px;
position:absolute;
left:988px;
top:2025px;
}


.imagem-profile6{
position:absolute;
left:1187px;
top:1815px;
}

.nome-kathle{
color: #ff4e5b;
text-decoration: none;
font-weight: 700;
font-style: normal;
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:1188px;
top:2000px;
}

.age-kathle{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #b6b6b6;
font-size: 14px;
line-height: 2;
letter-spacing: 0px;
position:absolute;
left:1188px;
top:2025px;
}

.imagem-uniting{
position:absolute;
left:0px;
top:2143px;
width:100%;
height:573px;
}

.imagem-casal-uniting{
position:absolute;
left:187px;
top:2233px;
width:776px;
}

.titulo-uniting1{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 60px;
line-height: 1.2;
letter-spacing: 0px;
text-shadow: 5px 5px 15px rgb(0 0 0 / 70%);
position:absolute;
left:918.6px;
top:2348px;
}

.titulo-uniting2{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 60px;
line-height: 1.2;
letter-spacing: 0px;
text-shadow: 5px 5px 15px rgb(0 0 0 / 70%);
position:absolute;
left:688px;
top:2420px;
}

.botao-uniting{
font-family: 'Ubuntu', sans-serif;
font-weight: 400;
font-style: normal;
color: #f7f7f7;
background-color: #ff4e5b;
border-color: transparent;
border-radius: 90px;
width:201px;
height:60px;
font-size: 18px;
line-height: 24px;
text-align: center;
cursor: pointer;
position:absolute;
left:1041px;
top:2552px;
}


.titulo-advantages{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 36px;
line-height: 1.2;
letter-spacing: 0px;
position:absolute;
left:634.1px;
top:2876px;
}

.icon-mundo{
position:absolute;
left:281px;
top:2970px;
width:82.3px;
height:82.4px;
}

.texto-mundo{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 18px;
line-height: 1.3;
letter-spacing: 0px;
position:absolute;
left:221.7px;
top:3073px;
width:13%;
text-align: center;
}

.icon-lupa{
position:absolute;
left:589px;
top:2978px;
width:72px;
height:72px;
}

.texto-lupa{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 18px;
line-height: 1.3;
letter-spacing: 0px;
position:absolute;
left:521.7px;
top:3073px;
width:13%;
text-align: center;
}

.icon-flexible{
position:absolute;
left:881px;
top:2970px;
width:83px;
height:83px;
}

.texto-flexible{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 18px;
line-height: 1.3;
letter-spacing: 0px;
position:absolute;
left:821.7px;
top:3073px;
width:13%;
text-align: center;
}


.icon-flexible{
position:absolute;
left:881px;
top:2970px;
width:83px;
height:83px;
}

.texto-flexible{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 18px;
line-height: 1.3;
letter-spacing: 0px;
position:absolute;
left:821.7px;
top:3073px;
width:13%;
text-align: center;
}

.icon-built{
position:absolute;
left:1181px;
top:2970px;
width:83px;
height:83px;
}

.texto-built{
font-weight: 400;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 18px;
line-height: 1.3;
letter-spacing: 0px;
position:absolute;
left:1121.7px;
top:3073px;
width:13%;
text-align: center;
}


.titulo-testimunha{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 36px;
line-height: 1.2;
letter-spacing: 0px;
position:absolute;
left:663.3px;
top:3300px;
}



* {
box-sizing: border-box;
padding: 0;
margin: 0;
}

html {
font-size: calc(5px + 0.4vw);
}

/* body {

} */

a {
text-decoration: none;
}

.intro {
position: relative;
width: 100%;
height: 100vh;
}

/* .left {
height: 100%;
width: 60%;
padding: 3rem 3rem 3rem 5rem;
display: table;
} */

/* .left > div {
display: table-cell;
vertical-align: middle;
} */

/* span {
color: #E8CA2B;
font-size: 14px;
font-weight: bold;
letter-spacing: 2px;
display: inline-block;
text-transform: uppercase;
font-family: sans-serif;
margin-bottom: 4rem;
} */


/* h1 {
font-size: 8rem;
margin-bottom: 3rem;
}
h1 + p {
color: #949494;
font-size: 1.6rem;
margin-bottom: 4rem;
}
p + a {
font-size: 1.6rem;
color: #000;
} */


.slider {
position: relative;
width:78%;
height: 100%;
left:199.3px;
top:2249px;
}


.slider .li {
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
background-size: cover;
background-repeat: no-repeat;
background-position: 50% 50%;
transition: clip .7s ease-in-out, z-index 0s .7s;
clip: rect(0, 100vw, 100vh, 100vw);
display: table;
}


/* .center-y {
display: table-cell;
vertical-align: middle;
text-align: center;
} */


.testimunha1{
position:absolute;
left:181px;
top:423px;
height:86px;
width:782px;
}


.nome-judi{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:512px;
top:532px;
}


.aspas1{
width:27px;
height:27px;
position:absolute;
left:216px;
top:597px;
}

.texto-judi{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:268.4px;
top:593px;
text-align: center;
}

.effective{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:832.8px;
top:593px;
text-align: center;
}

.texto-staff{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:713.6px;
top:629px;
text-align: center;
}



.texto-judi2{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:190px;
top:629px;
text-align: center;
}


.texto-judi3{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:372px;
top:665px;
text-align: center;
}

.texto-friend{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:694px;
top:665px;
text-align: center;
}


.testimunha2{
position:absolute;
left:181px;
top:423px;
height:86px;
width:782px;
}


.nome-kenneth{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:497.5px;
top:531px;
}


.aspas2{
width:27px;
height:27px;
position:absolute;
left:216px;
top:597px;
}

.texto-kenneth1{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:268.4px;
top:593px;
text-align: center;
}

.texto-give{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:835px;
top:593px;
text-align: center;
}

.texto-kenneth2{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:291.5px;
top:629px;
text-align: center;
}

.texto-goosebum{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:291.5px;
top:629px;
text-align: center;
}

.texto-have{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:796.2px;
top:629px;
text-align: center;
}


.testimunha3{
position:absolute;
left:181px;
top:423px;
height:86px;
width:782px;
}


.nome-adam{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:513.9px;
top:532px;
}


.aspas3{
width:27px;
height:27px;
position:absolute;
left:207px;
top:597px;
}

.texto-adam1{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:259.4px;
top:593px;
text-align: center;
}

.texto-adam2{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:185.3px;
top:629px;
text-align: center;
}

.texto-your-site{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:671.5px;
top:629px;
text-align: center;
}

.texto-added{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:809px;
top:593px;
text-align: center;
}

.texto-adam3{
font-weight: 400;
font-style: italic;
font-family: 'Ubuntu', sans-serif;
color: #000000;
font-size: 24px;
line-height: 1.5;
letter-spacing: 0px;
position:absolute;
left:451px;
top:665px;
text-align: center;
}



.li.current h3, .li.current h3 + a {
opacity: 1;
transition-delay: 1s;
transform: translate3d(0, 0, 0);
}


.li.current {
z-index: 1;
clip: rect(0, 100vw, 100vh, 0);
}


.li.prev {
clip: rect(0, 0, 100vh, 0);
}


.slider nav {
position: absolute;
bottom: 5%;
left:-60px;
top:727.5px;
right: 0;
text-align: center;
z-index: 10;
}


nav .a {
display: inline-block;
border-radius: 50%;
width: 1rem;
height: 1rem;
min-width: 12px;
min-height: 12px;
background: #d1d1d1;
margin: 0 0.4rem;
transition: transform .3s;
}

.a.current_dot {
transform: scale(1.5);
background:#ff4e5b;
}



@media screen and (max-width: 700px) {
.left {
width: 100%;
height: 30%;
}

.slider {
width:100%;
height:100%;
position:absolute;
left:0px;
top:2414px;
}

.testimunha1{
width:420px;
height:44px;
position: absolute;
left:12px;
top:238px;
}

.nome-judi{
position: absolute;
left:172.3px;
top:303px;
font-size: 15px;
}

.aspas1{
position:absolute;
left:17px;
top:351px;
width:19px;
height:18px;
}

.texto-judi{
position:absolute;
left:52.3px;
top:348px;
font-size: 16px;
/* width:84%; */
text-align: left;
}

.effective{
position:absolute;
left:16.5px;
top:372px;
font-size: 16px;
/* width:84%; */
text-align: left;
}

.texto-judi2{
position:absolute;
left:82px;
top:372px;
font-size: 16px;
/* width:84%; */
text-align: left;
}

.texto-staff{
position:absolute;
left:34.4px;
top:396px;
font-size: 16px;
/* width:84%; */
text-align: left;
}

.texto-judi3{
position:absolute;
left:198.5px;
top:396px;
font-size: 16px;
/* width:84%; */
text-align: left;
}

.texto-friend{
position:absolute;
left:196px;
top:420px;
font-size: 16px;
/* width:84%; */
text-align: left;
}


.testimunha2{
width:420px;
height:44px;
position: absolute;
left:12px;
top:238px;
}

.nome-kenneth{
position: absolute;
left:160px;
top:303px;
font-size: 15px;
}

.aspas2{
position:absolute;
left:17px;
top:351px;
width:19px;
height:18px;
}

.texto-kenneth1{
position:absolute;
left:51.4px;
top:348px;
font-size: 16px;
/* width:86%; */
text-align: left;
}

.texto-give{
position:absolute;
left:23.3px;
top:372px;
font-size: 16px;
/* width:84%; */
text-align: left;
}

.texto-goosebum{
position:absolute;
left:87.8px;
top:372px;
font-size: 16px;
/* width:84%; */
text-align: left;
}

.texto-have{
position:absolute;
left:203.2px;
top:396px;
font-size: 16px;
/* width:84%; */
text-align: left;
}


.testimunha3{
width:420px;
height:44px;
position: absolute;
left:12px;
top:238px;
}

.nome-adam{
position: absolute;
left:173.7px;
top:303px;
font-size: 15px;
}

.aspas3{
position:absolute;
left:22px;
top:351px;
width:19px;
height:18px;
}


.texto-adam1{
position:absolute;
left:57px;
top:348px;
font-size: 16px;
/* width:86%; */
text-align: left;
}

.texto-added{
position:absolute;
left:18.3px;
top:372px;
font-size: 16px;
/* width:86%; */
text-align: left;
}

.texto-adam2{
position:absolute;
left:105.3px;
top:372px;
font-size: 16px;
/* width:86%; */
text-align: left;
}


.texto-your-site{
position:absolute;
left:44px;
top:396px;
font-size: 16px;
/* width:86%; */
text-align: left;
}


.texto-adam3{
position:absolute;
left:238.7px;
top:396px;
font-size: 16px;
/* width:86%; */

}



.slider nav {
position: absolute;
bottom: 5%;
left:1px;
top:460px;
right: 0;
text-align: center;
z-index: 10;
}


nav .a {
display: inline-block;
border-radius: 50%;
width: 1rem;
height: 1rem;
min-width:9px;
min-height:9px;
background: #d1d1d1;
margin: 0 0.8rem;
transition: transform .3s;
}

.a.current_dot {
transform: scale(1.5);
background:#ff4e5b;
}

}

.imagem-roda{
position:absolute;
left:0px;
top:3860px;
width:100%;
height:359px;
}

.imagem-origame{
position:absolute;
left:187px;
top:3950px;
/* min-width: 180px; */
width:370px;
/* overflow: hidden;
position: relative; */
width: 371px;
aspect-ratio: auto 371 / 247;
height:197px;
-webkit-text-size-adjust: none;
}


.quadrado-imagem{
width:54px;
height:54px;
border: 2px solid #fff;
box-shadow: 0 1px 6px rgb(0 0 0 / 50%);
position:absolute;
left:195px;
top:3958px;
}

.titulo-origame{
font-family: 'Roboto', sans-serif;
position:absolute;
left:253px;
top:3960px;
color:#fff;
font-size:18px;
white-space: nowrap;
}

.imagem-origame-quadrado{
/* position:absolute;
left:187px;
top:3950px; */
height: 50px;
width: 50px;
}


.imagem-unitingres{
visibility: hidden;
position:absolute;
left:0px;
position:absolute;
left:0px;
top:2143px;
width:100%;
height:573px;
}


.retangulo-follow{
width:104px;
height:22px;
position:absolute;
left:196px;
top:4049px;
background-color: #fff;
z-index: 9999;
cursor: pointer;
}

.imagem-face{
position:absolute;
left:8px;
top:5px;
width:12px;
height:12px;
}

.titulo-follow{
font-size: 12px;
color: #4b4f56;
font-family: 'Roboto', sans-serif;
position:relative;
left:24px;
top:4px;
}


.retangulo-share{
width:63px;
height:22px;
position:absolute;
left:485px;
top:4049px;
background-color: #fff;
z-index: 9999;
cursor: pointer;
}

.imagem-share{
position:absolute;
left:8px;
top:3px;
width:14px;
height:15px;
}

.titulo-share{
font-size: 11px;
color: #4b4f56;
font-family: 'Roboto', sans-serif;
position:relative;
left:24.6px;
top:5px;
}

.contato-roda{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 24px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:721.3px;
top:3950px;
}

.icon-celular{
position:absolute;
left:717px;
top:4015px;
width:26px;
height:26px;
}

.numero-celular{
font-weight: 300;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:756px;
top:4015px;
}


.icon-email{
position:absolute;
left:720px;
top:4050px;
width:21px;
height:21px;
}

.arroba{
font-weight: 300;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ff4e5b;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:756px;
top:4048px;
}


.icon-pin{
position:absolute;
left:720px;
top:4085px;
width:21px;
height:21px;
}

.local{
font-weight: 300;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 18px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:756px;
top:4078px;
width:10%;
}


.segue-roda{
font-weight: 700;
font-style: normal;
font-family: 'Ubuntu', sans-serif;
color: #ffffff;
font-size: 24px;
line-height: 1.4;
letter-spacing: 0px;
position:absolute;
left:1088px;
top:3950px;
}

.icon-face{
position:absolute;
left:1081px;
top:4012px;
width:27px;
height:28px;
}

.icon-twitter{
position:absolute;
left:1122px;
top:4013px;
width:28px;
height:27px;
}

.icon-insta{
position:absolute;
left:1169.4px;
top:4014px;
width:24.1px;
height:24.2px;
}

.icon-pinte{
position:absolute;
left:1212px;
top:4014px;
width:24.1px;
height:23px;
}


@media (max-width: 690px) {
.menu {
width: 95%;
font-size: 24px;
}

.menu-item {
margin: .1em; 
}

.menu-item:nth-child(1) {
order: 0; 
}

.menu-item:nth-child(2) {
order: 1;
}

.menu-item:nth-child(3) {
order: 3; 
}

.menu-item:nth-child(4) {
order: 4; 
}


.menu-item:nth-child(5) {
order: 2; 
} 
}


@media (max-width: 480px) {


.imagem-cabecares, .imagem-unitingres, .imagem-rodares{
visibility: visible;
}

.icon-busca{
position: absolute;
left:414px;
top:72px;
width:15px;
height:15px;
}


.menu {
font-size: 12px; 
visibility: hidden;
}

.imagem-cabeca{
visibility: hidden;
}

.imagem-cabecares{
width:100%;
height:745px;
}

.retangulo-foto{
visibility: hidden;
}

.titulo1{
position: absolute;
left:16px;
top:120px;
font-size:30px;
}

.titulo2{
position: absolute;
left:103px;
top:120px;
font-size:30px;
}

.texto-titulo{
position: absolute;
left:16px;
top:160px;
font-size:12px;
}

.numero-registo{
position: absolute;
left:16px;
top:194px;
font-size: 22px;
}

.texto-register{
position: absolute;
left:16px;
top:220px;
font-size:13px;
}

.android{
position: absolute;
left:25px;
top:262px;
}

.apple{
position: absolute;
left:237px;
top:262px;
}

.casal-beijando{
position: absolute;
left:15px;
top:371px;
width:414px;
}

.titulo-find1{
position: absolute;
left:16px;
top:561px;
font-size: 27px;
}

.titulo-find2{
position: absolute;
left:16px;
top:593px;
font-size: 27px;
}

.botao-cabeca{
position: absolute;
left:15px;
top:666px;
width:134px;
height:46px;
font-size: 14px;
}

.imagem-welcome{
position: absolute;
left:15px;
top:830px;
width:414px;
}

.titulo-welcome{
position: absolute;
left:16px;
top:1221px;
font-size:26px;
}

.texto-welcome{
position: absolute;
left:16px;
top:1272px;
font-size:13px;
width:93%;
line-height: 19.4px;
}

.titulo-sobimagem-tired{
position: absolute;
left:16px;
top:1409px;
font-size:27px;
width: 80%;
}

.botao-welcome{
position: absolute;
left:15px;
top:1505px;
width: 121px;
height: 46px;
font-size: 14px;
}

.titulo-last{
position: absolute;
left:99.9px;
top:1606px;
font-size:26px;
}

.imagem-profile1{
position: absolute;
left:26px;
top:1677px;
}

.nome-donna{
position: absolute;
left:16px;
top:1857px;
font-size:15px;
}

.age-dona{
position: absolute;
left:16px;
top:1878px;
font-size:13px;
}


.imagem-profile2{
position: absolute;
left:248px;
top:1677px;
}

.nome-walter{
position: absolute;
left:238px;
top:1857px;
font-size:15px;
}

.age-walter{
position: absolute;
left:238px;
top:1878px;
font-size:13px;
}



.imagem-profile3{
position: absolute;
left:26px;
top:1924px;
}

.nome-sarah{
position: absolute;
left:16px;
top:2104px;
font-size:15px;
}

.age-sarah{
position: absolute;
left:16px;
top:2125px;
font-size:13px;
}


.imagem-profile4{
position: absolute;
left:248px;
top:1924px;
}

.nome-danielle{
position: absolute;
left:238px;
top:2104px;
font-size:15px;
}

.age-danielle{
position: absolute;
left:238px;
top:2125px;
font-size:13px;
}



.imagem-profile5{
position: absolute;
left:26px;
top:2171px;
}

.nome-john{
position: absolute;
left:16px;
top:2351px;
font-size:15px;
}

.age-john{
position: absolute;
left:16px;
top:2372px;
font-size:13px;
}


.imagem-profile6{
position: absolute;
left:248px;
top:2171px;
}

.nome-kathle{
position: absolute;
left:238px;
top:2351px;
font-size:15px;
}

.age-kathle{
position: absolute;
left:238px;
top:2372px;
font-size:13px;
}

.imagem-unitingres{
width:100%;
height:222px;
position: absolute;
left:0px;
top:2453px;
visibility:visible;
}

.imagem-uniting{
visibility: hidden;
width:100%;
height:222px;
position: absolute;
left:0px;
top:2453px;
}



.imagem-casal-uniting{
position: absolute;
left:15px;
top:2508px;
width:74.8%;
}

.titulo-uniting1{
position: absolute;
left:228px;
top:2538px;
font-size: 27px;
}

.titulo-uniting2{
position: absolute;
left:124.1px;
top:2570px;
font-size: 27px;
}

.botao-uniting{
position: absolute;
left:292px;
top:2623px;
width: 127px;
height: 46px;
font-size: 14px;
}

.titulo-advantages{
position: absolute;
left:122.5px;
top:2800px;
font-size: 26px;
}

.icon-mundo{
position: absolute;
left:197.4px;
top:2864px;
width:49.1px;
height:49.3px;
}

.texto-mundo{
position: absolute;
left:155.4px;
top:2934px;
font-size:13px;
width:30%;
}

.icon-lupa{
position: absolute;
left:202px;
top:2985.4px;
width:43px;
height:43px;
}

.texto-lupa{
position: absolute;
left:155.4px;
top:3050px;
font-size:13px;
width:30%;
}

.icon-flexible{
position: absolute;
left:197px;
top:3080px;
width:49px;
height:49px;
}

.texto-flexible{
position: absolute;
left:146.6px;
top:3150px;
font-size:13px;
width:34%;
}

.icon-built{
position: absolute;
left:197px;
top:3180px;
width:49px;
height:49px;
}

.texto-built{
position: absolute;
left:146.6px;
top:3250px;
font-size:13px;
width:34%;
}

.titulo-testimunha{
position: absolute;
left:143.5px;
top:3377px;
font-size:26px;
}

.imagem-roda{
visibility: hidden;
position: absolute;
left:0px;
top:3779px;
width:100%;
height:526px;
}


.imagem-rodares{
position: absolute;
left:0px;
top:3779px;
width:100%;
height:541px;
}

.quadrado-imagem{
position: absolute;
left:23px;
top:3842px;
}

.titulo-origame{
position: absolute;
left:81px;
top:3844px;
}


.imagem-origame{
position: absolute;
left:15px;
top:3788px;
width:413px;
height:192px;
/* aspect-ratio: auto 371 / 247; */
}

.retangulo-follow{
position: absolute;
left:24px;
top:3933px;
width:102px;
}

.retangulo-share{
position: absolute;
left:357px;
top:3933px;
width:63px;
}

.titulo-share{
width: 30%;
}

.contato-roda{
position: absolute;
left:16px;
top:4000px;
font-size: 20px;
}

.icon-celular{
position: absolute;
left:24px;
top:4050px;
width:17px;
height:17px;
}

.numero-celular{
position: absolute;
left:60.4px;
top:4048px;
font-size: 14px;
}


.icon-email{
position: absolute;
left:24.3px;
top:4075px;
width:16px;
height:16px;
}

.arroba{
position: absolute;
left:60.5px;
top:4074px;
font-size: 14px;
}

.icon-pin{
position: absolute;
left:24.3px;
top:4098px;
width:16.4px;
height:16px;
}

.local{
position: absolute;
left:60.5px;
top:4102px;
font-size: 14px;
width:53%;
}
 

.segue-roda{
position: absolute;
left:16px;
top:4157px;
font-size: 20px;
}
    
.icon-face{
position: absolute;
left:10px;
top:4203px;
width:22px;
height: 20px;
}

.icon-twitter{
position: absolute;
left:43px;
top:4203px;
width:21px;
height:21px;
}

.icon-insta{
position: absolute;
left:81px;
top:4204px;
width:18px;
height:18px;
}

.icon-pinte{
position: absolute;
left:115px;
top:4204px;
width:18px;
height:18px;
}

}
