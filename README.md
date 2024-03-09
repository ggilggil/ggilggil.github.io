
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>반짝반짝 버튼</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
        background-color: #f0f0f0; /* 배경색 추가 */
        transition: background-color 0.5s ease; /* 반짝이는 효과를 위한 트랜지션 */
    }
    button {
        padding: 10px 20px;
        margin: 10px;
        cursor: pointer;
        font-size: 16px;
        background-color: #3498db;
        color: #fff;
        border: none;
        border-radius: 5px;
        outline: none;
        transition: background-color 0.5s ease; /* 버튼 색상 전환을 위한 트랜지션 */
    }
    button:hover {
        background-color: #2980b9; /* 마우스 호버 시 버튼 색상 변경 */
    }
    button:active {
        animation: flash 0.5s ease; /* 버튼을 클릭할 때 반짝이는 애니메이션 적용 */
    }
    @keyframes flash {
        0%, 100% {
            background-color: #3498db;
        }
        50% {
            background-color: #f1c40f;
        }
    }
</style>
</head>
<body>

<h2>반짝반짝 버튼</h2>
<button>반짝</button>

</body>
</html>
