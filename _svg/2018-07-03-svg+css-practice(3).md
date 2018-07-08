---
title:  "svg+css实践-字体的移动和放大"
---

sidebar:
  nav: "docs"
---

<html>
	<head>
		<meta charset="UTF-8">
		<title>svg+css实践之字体的移动和放大</title>
	</head>
	<body>
	<p>这是一个使用了Bernard MT Condensed字体、颜色为紫色的字体，它的动画是一边移动一边放大</p>
	<svg xmlns="http://www.w3.org/2000/svg" width="945" height="709" viewBox="0 0 945 709">
  <g xmlns="http://www.w3.org/2000/svg" width="945" height="709" viewBox="0 0 945 709"> 
    <text id="TextElement" x="0" y="0" style="font-family:Bernard MT Condensed;font-size:24;fill: #800080;visibility:hidden" transform="rotate(0) scale(3 3)"> Look at me！
    <set attributeName="visibility" attributeType="CSS" to="visible" begin="1s" dur="5s" fill="freeze"/>
    <animateMotion path="M 0 0 L 100 100" begin="1s" dur="5s" fill="freeze"/>
    <animateTransform attributeName="transform" attributeType="XML" type="rotate" from="-30" to="0" begin="1s" dur="5s" fill="freeze"/> 
    <animateTransform attributeName="transform" attributeType="XML" type="scale" from="1" to="3" additive="sum" begin="1s" dur="5s" fill="freeze"/> 
    </text> 
  </g>
  </svg>
	</body>
</html>