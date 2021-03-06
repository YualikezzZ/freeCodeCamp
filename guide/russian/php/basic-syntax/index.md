---
title: Basic Syntax
localeTitle: Основной синтаксис
---
# Основной синтаксис

Сценарий PHP можно разместить где угодно в документе.

Сценарий PHP начинается с `<?php` и заканчивается на `?>`

Ниже приведен пример простого PHP-файла с PHP-скриптом, который использует встроенную функцию PHP «echo» для вывода текста «Привет мир!» на веб-странице

```
<html>
<body>

<h1>Моя первая страница PHP</h1>

<?php echo "Привет мир!"; ?>

</body>
</html> 
```

Будет выведено: 

```
Моя первая страница PHP

Привет, мир!
```

#### Заметка: PHP требует окончания инструкций точкой запятой (;). 
 
# Комментарии в PHP 
 
PHP поддерживает несколько способов комментирования: 
```
<!DOCTYPE html>
<html>
<body>

<?php
// Это однострочный комментарий

# Это так же однострочный комментарий

/*
Это многострочный комментарий
еще одна строка комментария
*/

// С их помощью вы можете комметировать код
$x = 5 /* + 15 */ + 5;
echo $x;
?>

</body>
</html>
```

# PHP Регистр символов 

Управляющие конструкции (if, else, while, итп), классы функции и пользовательские функции регистро НЕ зависимы.

В примере ниже, все три инструкции эквиваленты:
```
<!DOCTYPE html>
<html>
<body>

<?php
ECHO "Привет мир!<br>";
echo "Привет мир!<br>";
EcHo "Привет мир!<br>";
?>

</body>
</html>
```

### Имена переменных чувствительны к регистру символов. 

В примере ниже отобразиться только значение переменной $color (так как $color, $COLOR и $coLOR это разные переменные) 
```
<!DOCTYPE html>
<html>
<body>

<?php
$color = "красный";
echo "Мой портфель " . $color . "<br>";
echo "Мой дом " . $COLOR . "<br>";
echo "Мой телефон " . $coLOR . "<br>";
?>

</body>
</html>
```
