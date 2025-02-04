<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Слайды для Никитоса</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }
        .slide {
            display: none;
            text-align: center;
        }
        .slide.active {
            display: block;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
        }
        textarea {
            margin-top: 20px;
            width: 80%;
            height: 100px;
            font-size: 16px;
        }
    </style>
</head>
<body>

    <div class="slide active" id="slide1">
        <h1>Здарова Никитос!</h1>
        <button onclick="nextSlide()">Жми</button>
    </div>

    <div class="slide" id="slide2">
        <h1>👨🏿</h1>
        <textarea placeholder="Соси член"></textarea>
    </div>

    <script>
        function nextSlide() {
            document.getElementById('slide1').classList.remove('active');
            document.getElementById('slide2').classList.add('active');
        }
    </script>

</body>
</html>
