<!DOCTYPE html>
<html>
<head>
    <title>Простой веб сайт</title>
</head>
<body>
    <h1>Введите ссылку:</h1>
    <form action="#" method="get">
        <input type="text" name="url" placeholder="Введите ссылку">
        <input type="submit" value="Отправить">
    </form>

    <h2>Полученная ссылка:</h2>
    <p>
        <?php
            if(isset($_GET['url'])) {
                $url = $_GET['url'];
                echo $url;
            }
        ?>
    </p>
</body>
</html>
