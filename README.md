<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>무지개 색 반짝</title>
<style>
    body {
        background-color: pink;
        overflow: hidden;
        height: 100vh;
        position: relative;
    }

    .rainbow {
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        animation: none;
    }

    @keyframes rainbow {
        0% { background-color: red; }
        14% { background-color: orange; }
        28% { background-color: yellow; }
        42% { background-color: green; }
        57% { background-color: blue; }
        71% { background-color: indigo; }
        85% { background-color: violet; }
        100% { background-color: red; }
    }

    button {
        position: relative;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        padding: 15px 30px;
        font-size: 20px;
        background-color: #3498db;
        color: white;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        outline: none;
    }

    .counter {
        position: relative;
        top: 10px;
        right: 10px;
        font-size: 24px;
        color: white;
    }
</style>
</head>
<body>

<div class="rainbow"></div>
<button onclick="startRainbow()">배씨 머리</button>
<button onclick="startRainbow()">카운터 증가</button>
<div class="counter">0</div>

<script>
    var count = 0;
    var lastClickTime = 0;

    function startRainbow() {
        document.querySelector('.rainbow').style.animation = 'rainbow 3s infinite';
        setTimeout(function() {
            document.querySelector('.rainbow').style.animation = 'none';
        }, 3000); // 3초 후에 무지개 색 반짝 효과 사라지게 설정
    }

    function increaseCounter() {
        var currentTime = new Date().getTime();
        if (currentTime - lastClickTime <1000) {
            count += ㅋㅋ;
            document.querySelector('.counter').textContent = count;
        } else {
            count++;
            document.querySelector('.counter').textContent = count;
        }
        lastClickTime = currentTime;
    }
</script>
왜 옴?
</body>
</html>
