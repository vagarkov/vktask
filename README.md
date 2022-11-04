# WeatherAPP (React + TS + Redux toolkit)

React <br />
● Только функциональные компоненты <br />
● TypeScript везде, без использования типа Any <br />
● Локальное состояние не используется (useState), используется только
глобальное через Redux Toolkit <br />
● Интерфейс и стили любые, но интерфейс должен быть интуитивным и
наглядным <br />
● Базовые компоненты взять из Ant Design <br />
● При перезагрузке страницы или браузера сохраненные данные не должны
сбрасываться <br />


Тестовое задание <br />
Необходимо создать web-приложение для просмотра погоды. <br />
Данные необходимо получать из API https://yandex.com/dev/weather/. Тестовый доступ
дает делать 5000 запросов в день и получать прогноз погоды на 7 дней вперед.
По умолчанию данные о геопозиции берутся из данных о геопозиции браузера. Также
можно добавить новое местоположение через ручной ввод широты и долготы.<br />
<br />
Пользовательский сценарий
1. Пользователь заходит на страницу приложения
2. Приложение запрашивает доступ к геопозиции пользователя.
   a. Пользователь разрешает доступ к геопозиции. Переход к пункту 3.
   b. Пользователь не разрешает доступ к геопозиции. На странице
   показывается информация, что приложение не может определить
   геопозицию без этого разрешения. Предлагается нажать на кнопку
   “Разрешить доступ к данными геопозиции” и предоставить доступ.
   i. После нажатия на кнопку осуществляется переход к пункту 3.
3. На основе широты и долготы, взятой из информации по геопозиции,
   запрашивается текущая погода и прогноз на 7 дней вперед<br />
   <br />
   a. Отображается информация по текущему месту и погоде<br />
   i. Широта и долгота<br />
   ii. Название местности<br />
   iii. Местное время<br />
   iv. Температура<br />
   v. Температура (ощущается)<br />
   vi. Описание (солнечно, ветрено и т.д.)<br />
   vii. Скорость ветра<br />
   viii. Атмосферное давление<br />
   ix. Влажность<br />
   <br />
   b. Отображается прогноз на ближайшие 7 дней в виде вкладок между
   которыми можно переключаться. В каждой вкладке можно посмотреть:<br />
   i. Минимальную температуру<br />
   ii. Максимальную температуру<br />
   iii. Среднюю температуру за день<br />
   iv. Температура (ощущается)<br />
   v. Дату<br />
   vi. Описание (солнечно, ветрено и т.д.)<br />
   vii. Скорость ветра<br />
   viii. Атмосферное давление<br />
   ix. Влажность<br />
   <br />
4. Можно сохранить текущую геопозицию и присвоить ей свое название<br />
   <br />
5. Можно добавить новую геопозицию через заполнение формы из двух полей:
   широта и долгота. Таким образом можно посмотреть всю ту же информацию о
   погоде и прогнозе в другом месте и также сохранить эту геопозицию.<br />
   <br />
6. Пользователь должен иметь возможность переключаться между сохраненными
   геопозициями, редактировать их названия, удалять их.
   a. Если удалить все сохраненные геопозиции, то должна остаться только
   одна текущая (из данных геопозиции браузера)
