# plg_content_spnshare
Simple buttons on the site to share on social networks and messengers (plugin for Jommla CMS)

Плагин для кнопок поделиться в социальных сетях для сайта на CMS Joomla позволят выводить кнопки поделиться в социальных сетях  на страницах сайта. Основные преимущества модуля:

  - Плагин ставится на ваш сайт и не делает ни каких запросов для загрузки своей функциональности на сторонние сайты в отличии от большинства сторонних сервисов;
  - В плагине нет ничего лишнего в отличие от многих сторонних систем (можете сами посмотреть, какие и сколько сетевых запросов делают различные сторонние системы, которые очень часто не только обеспечивают вас функцией "поделиться" и но еще и сохраняют статистику запросов к сайту, например www.addthis.com. Вам это действительно нужно?).
   - Плагин не создает на страницах сайта внешних ссылок на сторонние сайты, включая и ссылки на сайты этих социальных сетей;
   - В плагине можно включить, при необходимости, отображение количества поделившихся. Но при этом надо учитывать, что хоть запрос на количество поделившихся социальной сети и делается по технологии ajax, и после отображения страницы сайта, все же это еще одни отдельный запрос на каждую социальную сеть. т.е. если вы включили отображение количества поделившихся в трех социальных сетях, то это добавит три ajax запроса (оно вам действительно необходимо?).

Установка плагина поделится в социальных сетях:

Для установки скачиваем архив plg_content_spnshare.zip и устанавливаем в joomla обычным образом. После установки  у вас появится выключенный плагин plg_content_spnshare.
Настройка плагина:

Вам необходимо зайти в плагин с делать следующее:

На закладке "Плагин" 

   - Задать ширину окна браузера в px, при которой боковое расположение кнопок будет переключаться на нижнее (по умолчаню стоит 1200. Условно, до 1200 - это смартфон, от 1200 - это десктоп);
   - Задать отступ от верха в px при срасположении кнопок сбоку (по умочанию стоит 100);
   - Задать использование minify (сжимает css и js);
   - Включить сам плагин.

На закладке "Описание" вы увидите просто краткое описание того, что надо сделать для настройки работы с плагином

На закладке "Кнопки" вы можете:

   - Включить необходимость отображения кнопки конкретной социальной сети;
   - Установить (изменить) порядок ее отображения;
   - Включить отображение количества поделившихся для конкретной социальной сети (доступно не по всем социальным сетям. Включайте, если это вам действительно необходимо, т.к. добавляется по запросу на каждую социальную сеть, хоть и ajax, но поисковики все это считают, да и зачем вам это?...).


Пример для Facebook:

Facebook                   Да/Нет

Порядок FB                   1

Поделившихся в FB   Да/Нет

Куда можно поделиться:

  - Facebook;
  - VK;
  - Twitter;
  - OK;
  - Мой Мир;
  - LinkedIn;
  - Pinterest;
  - LiveJournal;
  - Blogger;
  - Weibo;
  - Telegram;
  - WhatsApp;
  - Viber.

После установки плагина обязательно сделайте следующее:

   Создайте "пустой" модуль типа "HTML-код" (mod_custom) без какого либо html текста внутри и с произвольным наименованием в любой позиции, которая не будет создавать лишнего при его отображении (некоторые шаблоны умудряются сразу делать обрамление места, где ничего нет). Очень часто такие позиции называют типа "Debug";
   Включите сам модуль (на закладке "Модуль" параметр "Состояние" выставляется в "Опубликован");
   Отключите в модуле опцию печати заголовка (модуль ничего не должен выводить, даже заголовки... - параметр "Показывать заголовок" в "Скрыть");
   Разместите модуль на всех страницах сайта (на закладке "Привязка к пунктам меню" выберете опцию "На всех страницах");
   Включите в модуле опцию "Обрабатывать плагинами" (на закладке "Основные параметры").

Если в у вас включено кеширование на сайте, то лучше сбросьте кеш (кеш надо сбрасывать на mod_custom и com_content (или другой, если вы используется что-то другое для вывода контента, например k2)), что бы посмотреть, что у вас получилось.

Где посмотреть в живую плагин?

Посмотерть можно, например на https://hcproject.ru/ или https://iliantour.ru/

Где и как скачать плагин?

Плагин кнопок поделиться для Joomla можно скачать здесь и на странице загрузок http://seoprosto.net/other/download

Обновление плагина

В плагине присутствует проверка на выпуск новых версий. Как только появится новая версия, вы увидите соответствующее сообщение при работе в администраторе Joomla.
