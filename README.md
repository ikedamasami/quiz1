<!DOCTYPE HTML>
<html>
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
    <meta http-equiv="Content-Security-Policy" content="default-src * data: gap: content: https://ssl.gstatic.com; style-src * 'unsafe-inline'; script-src * 'unsafe-inline' 'unsafe-eval'">
    <script src="components/loader.js"></script>
    <link rel="stylesheet" href="components/loader.css">
    <link rel="stylesheet" href="css/style.css">
    <script>
        var answerList = [
            "✖️",
            "✖️",
            "✖️",
            "◯",
            "✖️"
        ];

        function showAnswer() {
            var choiceNo = document.getElementById("choiceList").value;
            document.getElementById("answer").innerHTML = "";
            document.getElementById("answer").innerHTML += "このクイズは、あなたの一般常識レベルがわかります。<br>";
            document.getElementById("answer").innerHTML += "あなたの答えは、「" + answerList[choiceNo] + "」です。"; 
        }
    </script>
</head>
<body>
	<h1>クイズ</h1>
	<p>日本国内で面積が一番小さい都道府県は？</p>
	<select id="choiceList">
		<option value="0">島根県</option>
		<option value="1">沖縄県</option>
		<option value="2">福井県</option>
		<option value="3">香川県</option>
		<option value="4">大阪府</option>
	</select>
	<button onclick="showAnswer()">回答する</button>
	<hr>
	<p id="answer"></p>
</body>
</html>
