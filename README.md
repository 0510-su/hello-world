<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title></title>
	</head>
	<body>
		<svg width="8cm" height="3cm" viewBox="0 0 800 300" version="1.1">
			<desc>基本动画元素</desc>
			<rect x="1" y=="1" width="798" height="298" fill="none" stroke="blue" stroke-width="2"/>
			<!--
                矩形位置和大小的动画
            -->
            <rect id="RectElement" x="300" y="100" width="300" height="100" fill="rgb(255,255,0)">
            	<animate attributeName="x" attributeType="XML" begin="0s" dur="9s" fill="freeze" from="300" to="0"/>
            	<animate attributeName="y" attributeType="XML" begin="0s" dur="9s" fill="freeze" from="100" to="0"/>
            	<animate attributeName="width" attributeType="XML" begin="0s" dur="9s" fill="freeze" from="300" to="800"/>
            	<animate attributeName="height" attributeType="XML" begin="0s" dur="9s" fill="freeze" from="100" to="300"/>
            </rect>
            <g transform="translate(100,100)">
            	<text id="TextElement" x="0" y="0" font-family="Verdana" font-size="35.27" visibility="hidden">
            		动画播放
            		<set attributeName="visibility" attributeType="CSS" to="visible" begin="3s" dur="6s" fill="freeze"/>
            		<aniamteMotion path="M 0 0 L 100 100" begin="3s" dur="6s" fill="freeze"/>
            		<animate attributeName="fill" attributeType="CSS" from="rgb(0,0,255)" to="rgb(128,0,0)" begin="3s" dur="6s" fill="freeze"/>
            		<animateTransform attributeName="transform" attributeType="XML" type="rotate" from="-30" to="0" begin="3s" dur="6s" fill="freeze"/>
            		<animateTransform attributeName="transform" attributeType="XML" type="scale" from="1" to="3" additive="sum" begin="3s" dur="6s" fill="freeze"/>
            		
            	</text>
            </g>
		</svg>
	</body>
	
	
</html>
