# Проект: Место (на React.js)
*Поделись с миром тем, что дорого тебе.*

**Функциональность:**

Всплывающие окна, редактирование профиля пользователя, добавление удаление картинок через сервер, постановка и сохранение лайка.

**Стек:**

БЭМ / HTML / CSS / JavaScript / NPM / Webpack / Babel / PostCSS / Git / REACT.JS / JSX

**Дизайн**
* Верстка приложения адаптивна для дисплеев с шириной от 320px до 1280px. Фото-карточки размещены с помощью GRID-сетки;
* Дизайн приложения выполнен по макету из Figma.

**Архитектура приложения**
* Именование и расположение файлов, папок, классов CSS, HTML-тегов выполнено по методологии БЭМ;
* CSS импортируются из корневого файла index.css.

**Скрипты/интеррактивность**
* В проекте реализована модульная система организации кода. Каждый модуль - это отдельный блок или функциональность сайта, созданный как `class`;
* Логика поведения блоков, элементов описана в `index.js`. Вспомогательные компоненты, константы импортируются в index.js из своих модулей. Местами используется гибридная(слабая) связь Классов для возможности их повторного переиспользования/добавления новых функций;
* Приложение подключено к серверу и обменивается информацией через асинхронные запросы `fetch()` в Api.js. C помощью API браузера приложение получает начальную информацию и в зависимости от поведения пользователя редактирует её (добавляет-удаляет карточки, ставит-удаляет лайки, меняет аватарку и описание пользователя). В случае ошибок при общении с сервером вы увидите сообщение в консоли браузера.

**Фрейм-ворки и сторонние библиотеки**
* Этот проект был портирован с Vanila.JS на рельсы React.JS;
* В приложении оттачивал хуки: useState, useEffect, useContext; 
* Настраивал ручное управление DOM-элементов в том числе через useRef;
* С помощью свойства `props.children` в компоненте `PopupWithForm` создал переиспользуемую форму;
* Приложение собирается Webpack с NPM библиотеками. В момент сборки происходит транспиляция JS кода, чтобы приложение работало на большинстве браузеров, в том числе предыдущих версий. Для CSS файлов применяется минификация через PostCSS, тем самым облегчаем css файл и автоматическии добавляем к свойствам префиксы для поддержки в различных браузерах.

**Среда разработки**
Проект сгенерирован с помощью Create React App.

**Действия для улучшения**
* Вернуть валидацию форм; 
* Изменение дизайна кнопки "Сохранить" при отправке данных на сервер. Добавить состояние "Готово" кнопки Submit в формах;
* Перелистывание карточек в popup zoomImage при помощи стрелочных кнопок на клавиатуре, экране;
* Отдельная страница "Избранное" для карточек с лайком пользователя.

## Инструкция по развёртыванию и системные требования
* 1. Скачайте ZIP-архив, распакуйте;
* 2. Откройте через VSCode или другой редактор кода;
* 3. Внутри директории проекта запустите `npm install`, это установит все зависимости данного проекта;
* 4. Запустите проект командой `npm start`.




