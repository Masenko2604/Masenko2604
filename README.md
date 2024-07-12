<div style="display: flex; justify-content: center; align-items: center;">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.herokuapp.com?font=Karla&weight=600&size=32&pause=1000&color=42EEF0&center=true&vCenter=true&random=false&width=435&lines=Welcome+to+my+profile+!;Hi%F0%9F%91%8B%2C+I'm+Tetyana;I+am+open+to+cooperation;I+continue+to+develop+;and+improve+my+skills." alt="Typing SVG" />
  </a>
<!-- <img src="https://raw.githubusercontent.com/matfantinel/matfantinel/master/waves.svg" width="100%" height="100" style="max-width: 100%;">
 </div> -->
//Pug
- var i = 0;
- var j = 0;
- var planes = 12;
- var spokes = 36;

// Sphere
.main-wrapper
  .sphere-wrapper
    while i < planes
      - i++
      .plane(class="plane-"+ i)
        - j = 0
        while j < spokes
          - j++
          .spoke(class="spoke-"+ j)
            .dot
//Less
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
  background: rgba(255, 255,255,1);
  left: -@dotSize/2;
  top: 100%;
  transform: rotateX(90deg);
}

.place-spokes(@spokes: @spokesNum; @i: 1) when (@i < @spokes) {
  @currDeg: unit((360 / @spokes * @i), deg);
  .spoke.spoke-@{i} {


Languages : 🇺🇦 Ukrainian - Native | ru Russian - Native | 🇬🇧 English - A2 | cz Czech - B2
- 📫 Email: **masyenko@gmail.com**
- 📄 Resume: **[https://github.com/Masenko2604/resume](https://masenko2604.github.io/resume/)**


<h3 align="left">Languages and Tools:</h3>
<p align="left">
 

<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Languages/javascript-original.svg" alt="Javascript" width="40" height="40"/>      
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Languages/typescript-original.svg" alt="Typescript" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Frontend/css3-original-wordmark.svg" alt="Css" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Frontend/react-original-wordmark.svg" alt="React" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Frontend/html5-original-wordmark.svg" alt="HTML" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Backend/nodejs-original-wordmark.svg" alt="NodeJs" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Frontend/redux-original.svg" alt="Redux" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Database/mongodb-original-wordmark.svg" alt="Mongodb" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Software/figma-icon.svg" alt="Figma" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Software/getpostman-icon.svg" alt="Postman" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/teamedwardforever/Readme-Generator/71f25dd8b98329b168142a6b782a107b75eab178/svg/Skills/Other/git-scm-icon.svg" alt="Git" width="40" height="40"/>
</p>





<div> <a href="https://github.com/Masenko2604" target="_blank"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" target="_blank"></a>
</div><h3 align="left">Stars</h3>
<img align="left" height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Masenko2604&layout=compact&theme=" alt=Masenko2604 />

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif"><h3 align="center">Statistics</h3>
<div align="center">
<a href="https://github.com/Masenko2604">
<img align="center" src="http://github-profile-summary-cards.vercel.app/api/cards/stats?username=Masenko2604&theme=2077" height="180em" />
<img align="center" src="http://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Masenko2604&theme=2077" height="180em" />
<img align="center" src="http://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Masenko2604&theme=2077" height="180em" />
<img align="center" src="http://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=Masenko2604&theme=2077" height="180em" />
<img align="center" src="http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Masenko2604&theme=2077" height="180em" />
</div>

 






















