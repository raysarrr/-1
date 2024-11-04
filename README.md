<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Дополнительные задания - Главная</title>
    <style>
        nav {
            position: fixed; 
            right: 0; 
            top: 50px; 
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
        }

        nav ul li {
            margin-bottom: 10px; 
        }

        nav ul li a {
            text-decoration: none;
            padding: 10px;
            border: 2px solid red;
            border-radius: 5px;
            color: black;
            background-color: white;
            display: block; 
            text-align: center;
        }

        nav ul li a.active {
            background-color: red;  
            color: white;          
        }

        nav ul li a:hover {
            background-color: red;
            color: white;
        }

        body {
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>

    <nav>
        <ul>
            <li><a href="index2.html">Главная</a></li>
            <li><a href="page1_2.html">Паспорт</a></li>
            <li><a href="page2_2.html">DOM_JS</a></li>
            <li><a href="page3_2.html">Задача</a></li>
            <li><a href="page4_2.html">Оригинальная задача</a></li>
        </ul>
    </nav>

    <h1>Дополнительные задания</h1>
    <p>Решения доп. заданий</p>

    <script>
     
        const currentLocation = location.href;

        const menuItem = document.querySelectorAll('nav ul li a');

        menuItem.forEach(item => {
            if (item.href === currentLocation) {
                item.classList.add('active'); 
            }
        });
    </script>
</body>
</html>
