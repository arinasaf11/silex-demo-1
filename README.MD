# Приложение на фреймворке Silex, размещённое на Heroku.
### 1. Форкаем [репозиторий](https://github.com/GossJS/silex-demo-1)
### 2. Рефакторинг кода index.php ветки middleware: добавляем дополнительные математические действия и авторство
```javascript
$app->get('/add/{n1}/{n2}', function ($n1, $n2) use($app) {
    return '<h2>Сумма: </h2><h3>' . ($n1 + $n2) . '</h3>'; 
  })->after($hdrs);
  $app->get('/sub/{n1}/{n2}', function ($n1, $n2) use($app) {
    return '<h2>Вычитание: </h2><h3>' . ($n1 - $n2) . '</h3>'; 
  })->after($hdrs);
  $app->get('/div/{n1}/{n2}', function ($n1, $n2) use($app) {
    return '<h2>Деление: </h2><h3>' . ($n1 / $n2) . '</h3>'; 
  })->after($hdrs);
  $app->get('/mul/{n1}/{n2}', function ($n1, $n2) use($app) {
    return '<h2>Умножение: </h2><h3>' . ($n1 * $n2) . '</h3>'; 
  })->after($hdrs);
  $app->get('/pow/{n1}/{n2}', function ($n1, $n2) use($app) {
    return '<h2>Возведение в степень: </h2><h3>' . ($n1 ** $n2) . '</h3>'; 
  })->after($hdrs);
  $app->get('/author', function () use($app) {
    return '<h4 id="author" title="GossJS">Arina Safiullina</h4>'; 
```
### 3. Деплоим приложение на heroku
### 4. Запускаем
![](https://github.com/arinasaf11/silex-demo-1/blob/master/Screenshot_0.png)
![](https://github.com/arinasaf11/silex-demo-1/blob/master/Screenshot_add.png)
![](https://github.com/arinasaf11/silex-demo-1/blob/master/Screenshot_div.png)
![](https://github.com/arinasaf11/silex-demo-1/blob/master/Screenshot_mul.png)
![](https://github.com/arinasaf11/silex-demo-1/blob/master/Screenshot_pow.png)
![](https://github.com/arinasaf11/silex-demo-1/blob/master/Screenshot_sub.png)
