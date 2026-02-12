<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<title>Алоха ❤️</title>

<style>
body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #ff9a9e, #fecfef);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
    overflow: hidden;
}

.container {
    background: white;
    padding: 35px;
    border-radius: 25px;
    box-shadow: 0 15px 40px rgba(0,0,0,0.2);
    max-width: 420px;
    animation: fadeIn 1s ease-in-out;
}

h1 {
    color: #ff4d6d;
}

button {
    padding: 12px 30px;
    margin: 10px;
    font-size: 18px;
    border: none;
    border-radius: 30px;
    cursor: pointer;
}

#yesBtn {
    background-color: #ff4d6d;
    color: white;
}

#noBtn {
    background-color: #ccc;
}

.hidden {
    display: none;
}

img {
    width: 170px;
    border-radius: 15px;
    margin: 10px;
}

@keyframes fadeIn {
    from {opacity: 0;}
    to {opacity: 1;}
}
</style>
</head>

<body>

<div class="container" id="question">
    <h1>Алоха ❤️<br><br>Ты хочешь стать моей валентинкой? 💌</h1>
    <button id="yesBtn">Да ❤️</button>
    <button id="noBtn">Нет</button>
</div>

<div class="container hidden" id="answer">
    <h1>Урааа ❤️</h1>

    <p>
        Алоха, я тебя очень сильно люблю ❤️<br><br>
        Ты моя любовь, и я поздравляю тебя с этим милым днем влюбленных.<br><br>
        Я благодарна тебе за всё, что ты делаешь для меня.<br>
        Благодарна вселенной, что ты появился в моей жизни.<br><br>
        Спасибо тебе ещё раз за всё ❤️<br><br>
        Ты до конца со мной, и я до конца с тобой.<br>
        Мы вечны ❤️❤️
    </p>

    <img src="https://i.imgur.com/2nCt3Sbl.jpg">
    <img src="https://i.imgur.com/eO9K8uXl.jpg">
</div>

<script>
const yesBtn = document.getElementById("yesBtn");
const noBtn = document.getElementById("noBtn");
const question = document.getElementById("question");
const answer = document.getElementById("answer");

yesBtn.onclick = function() {
    question.classList.add("hidden");
    answer.classList.remove("hidden");
}

noBtn.addEventListener("mouseover", function() {
    noBtn.style.position = "absolute";
    noBtn.style.left = Math.random() * (window.innerWidth - 100) + "px";
    noBtn.style.top = Math.random() * (window.innerHeight - 50) + "px";
});
</script>

</body>
</html>
