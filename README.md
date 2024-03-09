<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>폭죽 버튼</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
    }
    #fireworks {
        display: none;
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: 9999;
    }
</style>
</head>
<body>

<h2>폭죽 버튼</h2>
<button onclick="fireworks()">폭죽</button>

<div id="fireworks"></div>

<script>
    function fireworks() {
        var fireworks = document.getElementById("fireworks");
        fireworks.style.display = "block";

        setTimeout(function() {
            fireworks.style.display = "none";
        }, 5000); // 5초 후에 폭죽 효과 사라지게 설정
    }
</script>

</body>
</html>
