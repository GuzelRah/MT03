# Попарное тестирование
#### Для авторизации на сайт необходимо протестить следующие возможные варианты:
 __Username__
- standard_user
- locked_out_user
- problem_user
- performance_glitch_user
- неверное
- пустое  

__Password__
- secret_sauce
- неверное
- пустое

Путем ввода данных на сайте https://pairwise.teremokgames.com/ вывели следующие пары:

|№|Username|Password |
 |:--: |:--------  | :--------|
|1|standard_user |secret_sauce |
|2|standard_user| неверное |
|3|standard_user| пустое |
|4|locked_out_user | неверное |
|5|locked_out_user|пустое |
|6|locked_out_user| secret_sauce|
|7|problem_user  | пустое |
|8|problem_user  | secret_sauce|
|9|problem_user  | неверное |
|10|performance_glitch_user| secret_sauce|
|11|performance_glitch_user |неверное|
|12|performance_glitch_user | пустое|
|13|пустое|неверное|
|14|пустое | пустое|
|15|пустое  | secret_sauce|
|16|неверное  | пустое|
|17|неверное |secret_sauce|
|18|неверное |неверное|


### Тест кейсы для проверки авторизации на сайт

|ID|Заголовок |Предшествующие условия| Шаги | Ожидаемый результат|
|:--: |:--------  | :--------|:--------|:--------|
|01|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __standard_user__/ Password __secret_sauce__ |Открыта страница авторизации на сайт|В строке Username ввести __standard_user__. В строке Password ввести __secret_sauce__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|02|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __standard_user__/ Password __неверное значение__|Открыта страница авторизации на сайт|В строке Username ввести __standard_user__. В строке Password ввести  __неверное значение__. Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|03|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username  __standard_user__/ Password __пустое значение__|Открыта страница авторизации на сайт|В строке Username ввести __standard_user__. В строке Password ввести __пустое значение__. Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|04|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __locked_out_user__/Password __неверное значение__|Открыта страница авторизации на сайт|В строке Username ввести __locked_out_user__. В строке Password ввести __неверное значение__. Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|05|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __locked_out_user__/Password __пустое значение__ |Открыта страница авторизации на сайт|В строке Username ввести __locked_out_user__. В строке Password ввести __пустое значение__. Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|06|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __locked_out_user__/Password  __secret_sauce__ |Открыта страница авторизации на сайт|В строке Username ввести __locked_out_user__. В строке Password ввести __secret_sauce__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|07|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __problem_user__/Password	__пустое значение__ |Открыта страница авторизации на сайт|В строке Username __problem_user__ ввести. В строке Password ввести __пустое значение__. Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|08|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __problem_user__/Password	__secret_sauce__  |Открыта страница авторизации на сайт|В строке Username ввести __problem_user__. В строке Password ввести __secret_sauce__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|09|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __problem_user__/Password	__неверное значение__  |Открыта страница авторизации на сайт|В строке Username ввести __problem_user__. В строке Password ввести __неверное значение__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|10|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __performance_glitch_user__/Password	__secret_sauce__  |Открыта страница авторизации на сайт|В строке Username ввести __performance_glitch_user__. В строке Password ввести __secret_sauce__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|11|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __performance_glitch_user__/Password	__неверное значение__  |Открыта страница авторизации на сайт|В строке Username ввести __performance_glitch_user__. В строке Password ввести __неверное значение__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|12|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __performance_glitch_user__/Password	__пустое значение__  |Открыта страница авторизации на сайт|В строке Username ввести __performance_glitch_user__. В строке Password ввести __пустое значение__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|13|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __пустое значение__/Password	__неверное значение__  |Открыта страница авторизации на сайт|В строке Username ввести __пустое значение__. В строке Password ввести __неверное значение__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|14|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __пустое значение__/Password	__пустое значение__  |Открыта страница авторизации на сайт|В строке Username ввести __пустое значение__. В строке Password ввести __пустое значение__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|15|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __пустое значение__/Password	__secret_sauce__  |Открыта страница авторизации на сайт|В строке Username ввести __пустое значение__. В строке Password ввести __secret_sauce__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|16|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __неверное значение__/Password	__пустое значение__  |Открыта страница авторизации на сайт|В строке Username ввести __неверное значение__. В строке Password ввести __пустое значение__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|17|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __неверное значение__/Password	__secret_sauce__  |Открыта страница авторизации на сайт|В строке Username ввести __неверное значение__. В строке Password ввести __secret_sauce__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|
|18|Проверка авторизации на сайте https://www.saucedemo.com/ путем ввода Username __неверное значение__/Password	__неверное значение__  |Открыта страница авторизации на сайт|В строке Username ввести __неверное значение__. В строке Password ввести __неверное значение__ . Нажать на кнопку __LOGIN__|Ожидается авторизация на сайт|

