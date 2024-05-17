@radius: 300px;
@dotSize: 6px;
@spokesNum: 36;
@planesNum: 12;

html, body {
  margin: 0;
  padding: 0;
  height: 100%;
  overflow: hidden;
   background: #333;
}

.main-wrapper {
  display: flex;
  position: absolute;
	transform-style: preserve-3d;
	perspective: 400px;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  align-items: center;
  justify-content: center;
}
.sphere-wrapper {
	transform-style: preserve-3d;
  width: @radius;
  height: @radius;
  position: relative;
  // background: rgba(255,255,255,.1);
  // border-radius: 50%;
  animation: rotate3d 10s linear infinite;
}
.plane {
  position: absolute;
  transform-style: preserve-3d;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
}
.spoke {
  transform-origin: 0 0;
  transform-style: preserve-3d;
  position: absolute;
  left: 50%;
  top: 50%;
  height: @radius/2;
  width: 0px;
  }

.dot {
  position: absolute;
  width: @dotSize;
  height: @dotSize;
  border-radius: 50%;
  background: rgba(255,255,255,1);
  left: -@dotSize/2;
  top: 100%;
  }

.place-spokes(@spokes: @spokesNum; @i: 1) when (@i < @spokes) {
  @currDeg: unit((360 / @spokes * @i), deg);
  .spoke.spoke-@{i} {
    transform: rotateZ(@currDeg);
  }
  .place-spokes(@spokes; @i + 1);
}

.place-planes(@planes: @planesNum; @i: 1) when (@i < @planes) {
  @currDeg: unit(180 / @planes * @i, deg);
  .plane.plane-@{i} {
    transform: rotateY(@currDeg);
  }
  .place-planes(@planes; @i + 1);
}

.animate-dots(@spokes: @spokesNum/2; @i: 0) when (@i <= @spokes) {
  @delay: unit(@i/@spokes, s);
  @j: @spokesNum - @i;
  @colorDeg: unit(360/@spokesNum*@i, deg);
  .spoke-@{i} .dot, .spoke-@{j} .dot  {
    animation: pulsate .5s infinite @delay alternate both;
    background-color: spin(#f95, @colorDeg);
  }
  .animate-dots(@spokes, @i + 1);
}

.place-spokes();
.place-planes();
.animate-dots();

@keyframes rotate3d {
	  0% { transform: rotate3d(1,1,1,0deg)};
   25% { transform: rotate3d(1,1,1,90deg)};
   50% { transform: rotate3d(1,1,1,180deg)};
   75% { transform: rotate3d(1,1,1,270deg)};
	100% { transform: rotate3d(1,1,1,360deg)};
}

@keyframes pulsate {
    0% { transform: rotateX(90deg) scale(.3) translateZ(20px); }
  100% { transform: rotateX(90deg) scale(1) translateZ(0px); }
}

.animista-badge {
  font: normal 15px/1.5 sans-serif;
  position: absolute;
  right: 10px;
  bottom: 10px;
  color: rgba(255,255,255,.8);
  padding: .5em 1em;
}

a {
  color: #ff6060;
  text-decoration: none;
  &:hover { text-decoration: underline; }
}


<div> <a href="https://www.linkedin.com/in/https://www.linkedin.com/in/tetyana-masyenko-3533942a5/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>
<a href="https://github.com/https://github.com/Masenko2604/Masenko2604" target="_blank"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" target="_blank"></a>
<a href = "mailto:masyenko@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
</div><h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://linkedin.com/in/https://www.linkedin.com/in/tetyana-masyenko-3533942a5/" target="blank"><img align="center" src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Social/linked-in-alt.svg" alt="https://www.linkedin.com/in/tetyana-masyenko-3533942a5/" height="30" width="40" /></a></p>

<h3 align="left">Languages and Tools:</h3>
<p align="left">
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Languages/javascript-original.svg" alt="Javascript" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Frontend/react-original-wordmark.svg" alt="React" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Frontend/css3-original-wordmark.svg" alt="Css" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Frontend/html5-original-wordmark.svg" alt="HTML" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Languages/typescript-original.svg" alt="Typescript" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Backend/nodejs-original-wordmark.svg" alt="NodeJs" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Database/mongodb-original-wordmark.svg" alt="Mongodb" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Software/getpostman-icon.svg" alt="Postman" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Software/figma-icon.svg" alt="Figma" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Other/git-scm-icon.svg" alt="Git" width="40" height="40"/>
</p>






