<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>반짝반짝</title>
<style>
    body {
        background-color: black;
        overflow: hidden;
    }

    .blink {
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        background-color: white;
        animation: blink 0.5s infinite alternate;
    }

    @keyframes blink {
        from {
            opacity: 0;
        }
        to {
            opacity: 1;
        }
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

<div class="blink"></div>
<button onclick="blink()">반짝</button>

<script>
    function blink() {
        document.querySelector('.blink').style.display = 'block';
        setTimeout(function() {
            document.querySelector('.blink').style.display = 'none';
        }, 1000); // 1초 후에 반짝 효과 사라지게 설정
    }
</script>

</body>
</html>
