<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>무지개 색 반짝</title>
<style>
    body {
        background-color: black;
        overflow: hidden;
        height: 100vh;
    }

    .rainbow {
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        display: none;
        animation: rainbow 3s infinite;
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
        position: absolute;
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
</style>
</head>
<body>

<div class="rainbow"></div>
<button onclick="startRainbow()">무지개 색 반짝</button>

<script>
    function startRainbow() {
        document.querySelector('.rainbow').style.display = 'block';
        setTimeout(function() {
            document.querySelector('.rainbow').style.display = 'none';
        }, 3000); // 3초 후에 무지개 색 반짝 효과 사라지게 설정
    }
</script>

</body>
</html>
