<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>무지개 색 반짝</title>
<style>
    body {
        background-color: pink ;
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
<button onclick="startRainbow()">빤짝이_배</button>
<button onclick="startRainbow()">카운터_증가</button>
<div class="counter">0</div>

<script>
    var count = 1;
    var lastClickTime = 0;

    function rainbow(빤짝이_배) {
        document.querySelector('.rainbow').style.animation = 'rainbow 3s infinite';
        setTimeout(function() {
            document.querySelector('.rainbow').style.animation = 'none';
        }, 3000); // 3초 후에 무지개 색 반짝 효과 사라지게 설정
    }

    function increasecount(카우터_증가) {
        var currentTime = new Date().getTime();
        if (currentTime - lastClickTime <500) {
            count += 1;
            document.querySelector('.counter').textContent = count;
        } else {
            count++;
            document.querySelector('.counter').textContent = count;
        }
        lastClickTime = currentTime;
    }
</script>
왜 옴?
wö xing shi

워싱시

wú lun hé shí yù nì xiāng shí wö dou zhíg

우 룬 허스 위니 샹스 워 또우 즈

wö xing shi

워싱시

zhi Fi xié cí you rú jùn mã zài Fên chí

즈 삐 시에 츠 요우 루 쥔 마 짜이 뻔 츼

wö xing shi

워싱시

xin wäng shén chí zhi Fi zài yi luò Fi zhí

진 빵 션 츠 즈 삐 짜이 이 루어 삐 즈

wö xing shi

워싱시

gão jie yuàn shí rén rú qí ming hën wù shí

까오 지에 위앤 스 런 루 치 밍 헌 우 츠

Shí, Fù jù fēng fēi shā

시, 뿌 쥐 펑 페이 사

Shí, zhòngrén Fǎ nǐ kuā

시, 쫑 런 빠 니 쿠아

Shí, zhòng xīng shǒuhù de

시, 종 싱 셔우 후 타

Shí, rén zhōng cáizǐ jiā

시, 륀 종 차이 쯔 지아

Shí, yīlù zài qián xíng

시, 이 루 짜이 치앤 싱

Shí, yīshēng zhùdìng yíng

시, 이 셩 주 띵 잉

Shí, fēngyǔ jiē huì píng

시 펑 위 지에 훼이 핑

Shí, yángfān zài yángmíng

시, 양 판 짜이 양 밍

2절

Wǒ xìng cáo, zìzàì xiāoyáo yīshēn zhèngyì dǎnqì háo

워 싱 차오, 쯔 짜이 샤오 야오 이 션 정 이 딴 치 하오

Wǒ xìng cáo, cānghǎi jì liào jiǔ tuō shì wǒ de sùmiáo

워씽차오, 창 하이 지 랴오 싸 투어 스 워 더 쑤 먀오

Wǒ xìng cáo, shēnzhe zhàn páo guàshuài chūzhēng jù cháng máo

워씽차오, 신주어 잔 파오 꾸아 솨이 츄청 꾸어잔 마오

Wǒ xìng cáo, dírén āi huì yǒng guàn sānjūn dí Fài táo

워씽차오, 워 싱 차오, 띠 증 아이 하오 용 꾸안 싼 쥔 띠 빠이 타오
</body>
