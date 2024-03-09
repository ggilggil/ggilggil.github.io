# ggilggil.github.io
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>간단한 계산기</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
    }
    input[type="number"] {
        width: 100px;
        margin: 10px;
    }
    button {
        padding: 10px 20px;
        margin: 10px;
        cursor: pointer;
    }
</style>
</head>
<body>

<h2>간단한 계산기</h2>
<input type="number" id="num1">
<input type="number" id="num2">

<br><br>

<button onclick="add()">덧셈</button>
<button onclick="subtract()">뺄셈</button>
<button onclick="multiply()">곱셈</button>
<button onclick="divide()">나눗셈</button>

<p id="result"></p>

<script>
    function add() {
        let num1 = parseFloat(document.getElementById('num1').value);
        let num2 = parseFloat(document.getElementById('num2').value);
        document.getElementById('result').innerHTML = num1 + num2;
    }

    function subtract() {
        let num1 = parseFloat(document.getElementById('num1').value);
        let num2 = parseFloat(document.getElementById('num2').value);
        document.getElementById('result').innerHTML = num1 - num2;
    }

    function multiply() {
        let num1 = parseFloat(document.getElementById('num1').value);
        let num2 = parseFloat(document.getElementById('num2').value);
        document.getElementById('result').innerHTML = num1 * num2;
    }

    function divide() {
        let num1 = parseFloat(document.getElementById('num1').value);
        let num2 = parseFloat(document.getElementById('num2').value);
        if (num2 === 0) {
            document.getElementById('result').innerHTML = "0으로 나눌 수 없습니다.";
        } else {
            document.getElementById('result').innerHTML = num1 / num2;
        }
    }
</script>

</body>
</html>
