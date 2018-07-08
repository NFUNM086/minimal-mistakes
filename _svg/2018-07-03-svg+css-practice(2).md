---
title:  "svg+css实践-模仿进度条"

sidebar:
  nav: "docs"
---

<html>
	<head>
		<meta charset="UTF-8">
		<title>svg+css实践之模仿进度条</title>
	</head>
	<body>
	<p>这是一个描边颜色为黑色、填充颜色为黄色的矩形在逐渐变长</p>
		<svg>
    <rect x="10" y="10" width="200" height="20" stroke="black" fill="yellow">
  <animate
    attributeName="width"
    attributeType="XML"
    from="10" to="200"
    begin="0s" dur="5s"
    fill="freeze" />
    </rect>
        </svg>
	</body>
</html>