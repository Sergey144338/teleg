<?php
use yii\helpers\Url;
// Получаем параметр 'start' из GET-запроса
$start = Yii::$app->request->get('ref', '');

// Проверяем, является ли параметр числом
if (is_numeric($start)) {
    $startValue = $start; // Используем значение параметра, если это число
} else {
    $startValue = 1; // Если параметр не передан или не является числом, используем '1'
}

$link = Url::to("https://t.me/Zdorovievsem_bot?start=" . $startValue);
?>
<style>
    body {
        margin: 0;
        padding: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background: #ffffff !important;
        font-family: Arial, sans-serif;
        color: #6d6d6d !important;
    }

    .container {
        text-align: center;
    }

    .logo img {
        width: 100px; /* Ширина логотипа */
        height: 100px; /* Высота логотипа */
        margin-bottom: 20px;
        display: block;
        margin-left: auto;
        margin-right: auto;
        border-radius: 50px;
    }

    .title {
        font-size: 24px;
        margin-bottom: 20px;
    }

    .button {
        background-color: #36a3f7;
        color: white;
        padding: 10px 20px;
        text-decoration: none;
        border-radius: 5px;
        font-size: 18px;
        display: inline-block;
        margin-bottom: 20px;
    }

    .links {
        margin-top: 15px;
        font-size: 14px;
    }

    .footer {
        margin-top: 30px;
        font-size: 12px;
    }
</style>
<div class="container">
    <div class="logo">
        <img src="/images/logo.jpg" alt="Здоровье с doTERRA">
    </div>
    <div class="title">Здоровье с doTERRA</div>
    <a href="<?= htmlspecialchars($link) ?>" class="button">
        <img src="/images/telegram.png" alt="Icon" class="button-icon">
        Открыть в Telegram
    </a>
    <div class="footer">
        Нет программы Telegram? <a href="https://telegram.org/apps?setln=ru">Установите сейчас</a>
    </div>
</div>
