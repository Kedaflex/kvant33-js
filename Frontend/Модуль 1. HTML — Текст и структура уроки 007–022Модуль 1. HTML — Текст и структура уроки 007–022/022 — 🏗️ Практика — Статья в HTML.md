---
tags: [курс, модуль-1, урок, html, практика, статья, вёрстка, семантика]
урок: 22
модуль: 1
тема: "Практика — Статья в HTML"
длительность: 45 мин
---
# 022 — 🏗️ Практика — Статья в HTML

> [!info] Навигация
> ← [[021 — Спецсимволы и комментарии]] | [[023 — Простая таблица]] →

---

## 🎯 Цели урока

- Применить **все знания** модуля 1 в одном проекте
- Сверстать полноценную статью, используя все изученные теги
- Научиться планировать разметку **до** написания кода
- Получить готовый проект для портфолио

---

## 📖 Что будем делать

Мы сверстаем **энциклопедическую статью** о языке HTML — похожую на статью из Wikipedia. Она будет содержать все типы контента, которые мы изучили в модуле 1:

| Элемент | Какие теги используем |
|---|---|
| Структура документа | `<!DOCTYPE>`, `<html>`, `<head>`, `<body>`, мета-теги |
| Заголовки | `<h1>`, `<h2>`, `<h3>` |
| Текст | `<p>`, `<br>`, `<hr>` |
| Форматирование | `<strong>`, `<em>`, `<b>`, `<i>`, `<mark>`, `<del>`, `<ins>`, `<sub>`, `<sup>`, `<small>`, `<abbr>` |
| Ссылки | `<a>` с разными типами `href` |
| Изображения | `<img>`, `<figure>`, `<figcaption>` |
| Списки | `<ul>`, `<ol>`, `<dl>` |
| Цитаты и код | `<blockquote>`, `<q>`, `<cite>`, `<code>`, `<pre>`, `<kbd>` |
| Спецсимволы | `&lt;`, `&gt;`, `&amp;`, `&mdash;`, `&laquo;`, `&raquo;`, `&copy;`, `&nbsp;` |
| Комментарии | `<!-- -->` |

---

## 🗺️ Шаг 1: Планирование структуры

Прежде чем писать код, спланируем структуру статьи.

### Оглавление будущей статьи

| Уровень | Заголовок | Содержимое |
|---|---|---|
| h1 | HTML — язык разметки | — |
| h2 | Содержание | Якорные ссылки |
| h2 | Введение | Абзацы, определения, ссылки |
| h2 | История | Список дат, цитата |
| h3 | Ранние версии | Абзацы |
| h3 | Современный HTML5 | Абзацы, список |
| h2 | Основные понятия | Определения |
| h3 | Теги и элементы | Код, примеры |
| h3 | Атрибуты | Код, примеры |
| h2 | Пример кода | Блок кода |
| h2 | Связь с CSS и JavaScript | Изображение, список |
| h2 | Интересные факты | Маркированный список |
| h2 | Полезные ресурсы | Ссылки |
| h2 | Источники | Нумерованный список |
| — | Подвал | Копирайт |

> [!tip] Привычка планировать
> Профессиональные разработчики **всегда** планируют разметку до написания кода. Это экономит время и предотвращает хаотичную структуру.

---

## 📂 Шаг 2: Создание проекта

| Шаг | Действие |
|---|---|
| 1 | Создай папку `022-article` внутри `web-course` |
| 2 | Внутри создай папку `images` |
| 3 | Создай файл `index.html` |
| 4 | Скачай любую картинку (или используй заглушку) и сохрани в `images/` |
```text
📂 022-article/  
├── 📄 index.html  
└── 📂 images/  
└── 🖼️ html-css-js.png (или заглушка)
```

---

## 💻 Шаг 3: Пишем код

Набирай **вручную** — не копируй. Код разбит на секции с пояснениями.

```html
<!DOCTYPE html>
<html lang="ru">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML — язык разметки гипертекста</title>
  </head>
  <body>

    <!-- ==================== ЗАГОЛОВОК СТАТЬИ ==================== -->
    <h1 id="top"><abbr title="HyperText Markup Language">HTML</abbr>&nbsp;&mdash; язык разметки гипертекста</h1>

    <p>
      <small>
        Материал из учебного проекта
        &bull; Последнее обновление: <time datetime="2024-03-15">15&nbsp;марта&nbsp;2024</time>
      </small>
    </p>

    <hr>

    <!-- ==================== СОДЕРЖАНИЕ ==================== -->
    <nav>
      <h2 id="contents">Содержание</h2>
      <ol>
        <li><a href="#intro">Введение</a></li>
        <li><a href="#history">История</a>
          <ol type="a">
            <li><a href="#early">Ранние версии</a></li>
            <li><a href="#html5">Современный HTML5</a></li>
          </ol>
        </li>
        <li><a href="#concepts">Основные понятия</a>
          <ol type="a">
            <li><a href="#tags">Теги и элементы</a></li>
            <li><a href="#attributes">Атрибуты</a></li>
          </ol>
        </li>
        <li><a href="#example">Пример кода</a></li>
        <li><a href="#related">Связь с CSS и JavaScript</a></li>
        <li><a href="#facts">Интересные факты</a></li>
        <li><a href="#resources">Полезные ресурсы</a></li>
        <li><a href="#sources">Источники</a></li>
      </ol>
    </nav>

    <hr>

    <!-- ==================== ВВЕДЕНИЕ ==================== -->
    <h2 id="intro">Введение</h2>

    <figure>
      <img
        src="https://via.placeholder.com/700x300/e44d26/ffffff?text=HTML5"
        alt="Логотип HTML5 — оранжевый щит с цифрой 5"
        width="700"
        height="300"
      >
      <figcaption>Рис.&nbsp;1&nbsp;&mdash; Логотип HTML5</figcaption>
    </figure>

    <p>
      <strong><abbr title="HyperText Markup Language">HTML</abbr></strong>
      (от&nbsp;англ. <i>HyperText Markup Language</i>&nbsp;&mdash; &laquo;язык гипертекстовой
      разметки&raquo;)&nbsp;&mdash; стандартизированный язык разметки документов для просмотра
      веб-страниц в&nbsp;браузере. Веб-браузеры получают HTML-документ от&nbsp;сервера
      или из&nbsp;локального хранилища и&nbsp;отображают его в&nbsp;виде мультимедийной
      веб-страницы.
    </p>

    <p>
      HTML описывает <strong>структуру</strong> веб-страницы <em>семантически</em>,
      а&nbsp;также изначально включал инструкции по&nbsp;её&nbsp;внешнему виду.
      Наряду с&nbsp;<abbr title="Cascading Style Sheets">CSS</abbr>
      и&nbsp;JavaScript, HTML&nbsp;&mdash; одна из&nbsp;трёх основных технологий
      создания веб-страниц.
    </p>

    <dl>
      <dt>Расширение файлов</dt>
      <dd><code>.html</code>, <code>.htm</code></dd>

      <dt>Тип</dt>
      <dd>Язык разметки</dd>

      <dt>Разработчик</dt>
      <dd><abbr title="Web Hypertext Application Technology Working Group">WHATWG</abbr>,
        ранее&nbsp;&mdash; <abbr title="World Wide Web Consortium">W3C</abbr></dd>

      <dt>Текущая версия</dt>
      <dd>HTML Living Standard (постоянно обновляется)</dd>
    </dl>

    <!-- ==================== ИСТОРИЯ ==================== -->
    <h2 id="history">История</h2>

    <p>
      HTML был создан <strong>Тимом Бернерсом-Ли</strong> в&nbsp;<strong>1991&nbsp;году</strong>
      в&nbsp;исследовательском центре <abbr title="Conseil Européen pour la Recherche Nucléaire">ЦЕРН</abbr>
      (Женева, Швейцария). Первоначально HTML был разработан как средство для&nbsp;обмена
      научными документами между физиками разных стран.
    </p>

    <blockquote cite="https://www.w3.org/People/Berners-Lee/">
      <p>
        Я&nbsp;просто взял идею гипертекста и&nbsp;соединил её&nbsp;с&nbsp;идеей
        <abbr title="Transmission Control Protocol / Internet Protocol">TCP/IP</abbr>
        и&nbsp;системой доменных имён, и&nbsp;&mdash; <em>та-дам!</em>&nbsp;&mdash;
        появился Всемирный Веб.
      </p>
      <footer>&mdash; <cite>Тим Бернерс-Ли</cite>, создатель HTML и&nbsp;Всемирной паутины</footer>
    </blockquote>

    <!-- История: ранние версии -->
    <h3 id="early">Ранние версии</h3>

    <ol>
      <li><strong>1991</strong>&nbsp;&mdash; Тим Бернерс-Ли публикует первый документ с&nbsp;описанием 18&nbsp;тегов HTML</li>
      <li><strong>1995</strong>&nbsp;&mdash; HTML&nbsp;2.0 становится первым официальным стандартом</li>
      <li><strong>1997</strong>&nbsp;&mdash; HTML&nbsp;3.2 добавляет таблицы и&nbsp;апплеты</li>
      <li><strong>1999</strong>&nbsp;&mdash; HTML&nbsp;4.01&nbsp;&mdash; основной стандарт на&nbsp;долгие годы</li>
      <li><strong>2000</strong>&nbsp;&mdash; <abbr title="Extensible HyperText Markup Language">XHTML</abbr>&nbsp;1.0&nbsp;&mdash; попытка сделать HTML строже (на&nbsp;основе XML)</li>
    </ol>

    <!-- История: HTML5 -->
    <h3 id="html5">Современный HTML5</h3>

    <p>
      Работа над HTML5 началась в&nbsp;<strong>2004&nbsp;году</strong> группой
      <abbr title="Web Hypertext Application Technology Working Group">WHATWG</abbr>.
      Официально стандарт HTML5 был опубликован <abbr title="World Wide Web Consortium">W3C</abbr>
      в&nbsp;<strong>2014&nbsp;году</strong>.
    </p>

    <p>Основные нововведения HTML5:</p>

    <ul>
      <li>Семантические теги: <code>&lt;header&gt;</code>, <code>&lt;footer&gt;</code>,
        <code>&lt;nav&gt;</code>, <code>&lt;article&gt;</code>, <code>&lt;section&gt;</code></li>
      <li>Встроенное аудио и&nbsp;видео: <code>&lt;audio&gt;</code>, <code>&lt;video&gt;</code></li>
      <li>Элемент <code>&lt;canvas&gt;</code> для&nbsp;рисования графики</li>
      <li>Новые типы полей ввода: <code>date</code>, <code>email</code>, <code>range</code></li>
      <li>Поддержка <del>Flash</del> <ins>нативного мультимедиа</ins> (без плагинов)</li>
      <li>Геолокация, локальное хранилище, drag&amp;drop</li>
    </ul>

    <!-- ==================== ОСНОВНЫЕ ПОНЯТИЯ ==================== -->
    <h2 id="concepts">Основные понятия</h2>

    <!-- Теги и элементы -->
    <h3 id="tags">Теги и&nbsp;элементы</h3>

    <p>
      <strong>Тег</strong>&nbsp;&mdash; это команда для&nbsp;браузера, заключённая в&nbsp;угловые
      скобки. <strong>Элемент</strong>&nbsp;&mdash; это тег вместе с&nbsp;его содержимым.
    </p>

    <dl>
      <dt>Парные теги</dt>
      <dd>Имеют открывающую и&nbsp;закрывающую часть: <code>&lt;p&gt;Текст&lt;/p&gt;</code></dd>

      <dt>Одиночные теги</dt>
      <dd>Не&nbsp;имеют закрывающей части: <code>&lt;br&gt;</code>, <code>&lt;img&gt;</code>, <code>&lt;hr&gt;</code></dd>

      <dt>Вложенность</dt>
      <dd>Элементы могут находиться внутри других элементов. Правило: <mark>первым открыл&nbsp;&mdash; последним закрыл</mark></dd>
    </dl>

    <p>Пример правильной вложенности:</p>

    <pre><code>&lt;p&gt;Текст &lt;strong&gt;&lt;em&gt;жирный курсив&lt;/em&gt;&lt;/strong&gt; обычный.&lt;/p&gt;</code></pre>

    <!-- Атрибуты -->
    <h3 id="attributes">Атрибуты</h3>

    <p>
      <strong>Атрибуты</strong> добавляют тегам дополнительную информацию.
      Они пишутся в&nbsp;<em>открывающем</em> теге в&nbsp;формате
      <code>имя=&quot;значение&quot;</code>.
    </p>

    <p>Самые важные атрибуты:</p>

    <ul>
      <li><code>href</code>&nbsp;&mdash; адрес ссылки (<code>&lt;a&gt;</code>)</li>
      <li><code>src</code>&nbsp;&mdash; путь к&nbsp;файлу (<code>&lt;img&gt;</code>)</li>
      <li><code>alt</code>&nbsp;&mdash; альтернативный текст (<code>&lt;img&gt;</code>)</li>
      <li><code>class</code>&nbsp;&mdash; CSS-класс (любой тег)</li>
      <li><code>id</code>&nbsp;&mdash; уникальный идентификатор (любой тег)</li>
    </ul>

    <p>Пример тега с&nbsp;атрибутами:</p>

    <pre><code>&lt;a href=&quot;https://google.com&quot; target=&quot;_blank&quot;&gt;Google&lt;/a&gt;</code></pre>

    <!-- ==================== ПРИМЕР КОДА ==================== -->
    <h2 id="example">Пример кода</h2>

    <p>Минимальный HTML-документ выглядит так:</p>

    <pre><code>&lt;!DOCTYPE html&gt;
&lt;html lang=&quot;ru&quot;&gt;
  &lt;head&gt;
    &lt;meta charset=&quot;UTF-8&quot;&gt;
    &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt;
    &lt;title&gt;Моя страница&lt;/title&gt;
  &lt;/head&gt;
  &lt;body&gt;
    &lt;h1&gt;Привет, мир!&lt;/h1&gt;
    &lt;p&gt;Это моя первая веб-страница.&lt;/p&gt;
  &lt;/body&gt;
&lt;/html&gt;</code></pre>

    <p>
      Чтобы создать этот файл в&nbsp;VS&nbsp;Code, набери <kbd>!</kbd> и&nbsp;нажми
      <kbd>Tab</kbd>&nbsp;&mdash; Emmet сгенерирует шаблон автоматически.
    </p>

    <!-- ==================== СВЯЗЬ С CSS И JS ==================== -->
    <h2 id="related">Связь с&nbsp;CSS и&nbsp;JavaScript</h2>

    <p>HTML работает в&nbsp;связке с&nbsp;двумя другими технологиями:</p>

    <figure>
      <img
        src="https://via.placeholder.com/600x250/282c34/61dafb?text=HTML+%2B+CSS+%2B+JS"
        alt="Три технологии веба: HTML (структура), CSS (стили), JavaScript (поведение)"
        width="600"
        height="250"
        loading="lazy"
      >
      <figcaption>Рис.&nbsp;2&nbsp;&mdash; Три основные технологии веб-разработки</figcaption>
    </figure>

    <dl>
      <dt><strong><abbr title="HyperText Markup Language">HTML</abbr></strong></dt>
      <dd>Определяет <strong>структуру</strong> и&nbsp;<strong>содержимое</strong> страницы.
        Отвечает на&nbsp;вопрос: <q>Что на&nbsp;странице?</q></dd>

      <dt><strong><abbr title="Cascading Style Sheets">CSS</abbr></strong></dt>
      <dd>Определяет <strong>внешний вид</strong> страницы: цвета, шрифты, расположение элементов.
        Отвечает на&nbsp;вопрос: <q>Как это выглядит?</q></dd>

      <dt><strong>JavaScript</strong></dt>
      <dd>Определяет <strong>поведение</strong> страницы: реакция на&nbsp;клики, загрузка данных, анимации.
        Отвечает на&nbsp;вопрос: <q>Что это делает?</q></dd>
    </dl>

    <!-- ==================== ИНТЕРЕСНЫЕ ФАКТЫ ==================== -->
    <h2 id="facts">Интересные факты</h2>

    <ul>
      <li>Первая версия HTML содержала всего <strong>18&nbsp;тегов</strong>. Сейчас их&nbsp;около&nbsp;110</li>
      <li>HTML&nbsp;&mdash; это <em>не&nbsp;язык программирования</em>, а&nbsp;язык <em>разметки</em></li>
      <li>Символ <code>&amp;amp;</code> называется <i>амперсанд</i> (от&nbsp;лат. <i>et</i>&nbsp;&mdash; &laquo;и&raquo;)</li>
      <li>Самый посещаемый сайт в&nbsp;мире&nbsp;&mdash; <a href="https://google.com" target="_blank" rel="noopener noreferrer">Google</a>&nbsp;&mdash; тоже написан на&nbsp;HTML</li>
      <li>Площадь первого в&nbsp;мире веб-сайта составляла примерно 1&nbsp;000&nbsp;байт. Сегодня средняя веб-страница весит более 2&nbsp;<abbr title="мегабайт">МБ</abbr></li>
      <li>Тег <code>&lt;marquee&gt;</code> (бегущая строка) и&nbsp;<code>&lt;blink&gt;</code> (мигающий текст) были удалены из&nbsp;стандарта как <del>крутые</del> <ins>ужасные</ins> решения</li>
    </ul>

    <!-- ==================== ПОЛЕЗНЫЕ РЕСУРСЫ ==================== -->
    <h2 id="resources">Полезные ресурсы</h2>

    <ul>
      <li>
        <a href="https://developer.mozilla.org/ru/docs/Web/HTML" target="_blank" rel="noopener noreferrer">
          <cite>MDN Web Docs</cite>&nbsp;&mdash; HTML
        </a>&nbsp;&mdash; полная документация на&nbsp;русском языке
      </li>
      <li>
        <a href="https://htmlreference.io" target="_blank" rel="noopener noreferrer">
          <cite>HTML Reference</cite>
        </a>&nbsp;&mdash; визуальный справочник по&nbsp;всем тегам
      </li>
      <li>
        <a href="https://validator.w3.org" target="_blank" rel="noopener noreferrer">
          W3C Validator
        </a>&nbsp;&mdash; проверка HTML-кода на&nbsp;ошибки
      </li>
      <li>
        <a href="https://caniuse.com" target="_blank" rel="noopener noreferrer">
          Can I Use
        </a>&nbsp;&mdash; таблицы поддержки тегов и&nbsp;CSS-свойств браузерами
      </li>
    </ul>

    <!-- ==================== ИСТОЧНИКИ ==================== -->
    <h2 id="sources">Источники</h2>

    <ol>
      <li>
        <a href="https://html.spec.whatwg.org" target="_blank" rel="noopener noreferrer">
          HTML Living Standard
        </a>&nbsp;&mdash; официальная спецификация
        <sup><a href="#sources">[1]</a></sup>
      </li>
      <li>
        <a href="https://ru.wikipedia.org/wiki/HTML" target="_blank" rel="noopener noreferrer">
          Статья &laquo;HTML&raquo; в&nbsp;Википедии
        </a>
        <sup><a href="#sources">[2]</a></sup>
      </li>
      <li>
        <a href="https://www.w3.org/People/Berners-Lee/" target="_blank" rel="noopener noreferrer">
          Страница Тима Бернерса-Ли на&nbsp;сайте W3C
        </a>
        <sup><a href="#sources">[3]</a></sup>
      </li>
    </ol>

    <hr>

    <!-- ==================== НАВИГАЦИЯ ==================== -->
    <p>
      <a href="#top">&uarr;&nbsp;Вернуться к&nbsp;началу</a>
      &nbsp;&bull;&nbsp;
      <a href="#contents">К&nbsp;содержанию</a>
    </p>

    <hr>

    <!-- ==================== ПОДВАЛ ==================== -->
    <footer>
      <p>
        <small>
          &copy; 2024 Учебный проект.
          Создано в&nbsp;рамках курса &laquo;Основы веб-разработки&raquo;.
          <br>
          Автор: <a href="mailto:student@example.com">student@example.com</a>
          &nbsp;&bull;&nbsp;
          Телефон: <a href="tel:+79001234567">+7&nbsp;(900)&nbsp;123-45-67</a>
        </small>
      </p>
    </footer>

  </body>
</html>
````

---

## ✅ Шаг 4: Чек-лист — что должно быть в статье

Проверь, что твоя статья содержит **все** элементы:

### Структура

|Элемент|Есть?|
|---|---|
|`<!DOCTYPE html>`|⬜|
|`<html lang="ru">`|⬜|
|`<meta charset="UTF-8">`|⬜|
|`<meta name="viewport" ...>`|⬜|
|`<title>` с осмысленным текстом|⬜|

### Заголовки

|Элемент|Есть?|
|---|---|
|Один `<h1>`|⬜|
|Несколько `<h2>`|⬜|
|Минимум два `<h3>`|⬜|
|Правильная иерархия (без пропусков)|⬜|

### Текст

|Элемент|Есть?|
|---|---|
|Абзацы `<p>`|⬜|
|`<strong>` (важный текст)|⬜|
|`<em>` (смысловое ударение)|⬜|
|`<b>` или `<i>`|⬜|
|`<mark>` (выделение)|⬜|
|`<del>` + `<ins>` (удаление + вставка)|⬜|
|`<sub>` или `<sup>`|⬜|
|`<small>` (мелкий текст)|⬜|
|`<abbr>` с `title`|⬜|

### Ссылки

|Элемент|Есть?|
|---|---|
|Внешние ссылки с `target="_blank"`|⬜|
|Якорные ссылки (навигация внутри страницы)|⬜|
|Ссылка на email `mailto:`|⬜|
|Ссылка на телефон `tel:`|⬜|
|Ссылка «Вернуться наверх»|⬜|

### Изображения

|Элемент|Есть?|
|---|---|
|`<img>` с `src`, `alt`, `width`, `height`|⬜|
|`<figure>` + `<figcaption>`|⬜|
|`loading="lazy"` хотя бы на одной картинке|⬜|

### Списки

|Элемент|Есть?|
|---|---|
|Маркированный `<ul>`|⬜|
|Нумерованный `<ol>`|⬜|
|Список определений `<dl>`|⬜|
|Вложенный список|⬜|

### Цитаты и код

|Элемент|Есть?|
|---|---|
|`<blockquote>` с `<footer>` и `<cite>`|⬜|
|`<q>` (строчная цитата)|⬜|
|`<code>` (строчный код)|⬜|
|`<pre><code>` (блок кода)|⬜|
|`<kbd>` (клавиши)|⬜|

### Спецсимволы и комментарии

|Элемент|Есть?|
|---|---|
|`&lt;`, `&gt;`, `&amp;`|⬜|
|`&nbsp;` (неразрывный пробел)|⬜|
|`&mdash;` (длинное тире)|⬜|
|`&laquo;` и `&raquo;` (кавычки-ёлочки)|⬜|
|`&copy;` (копирайт)|⬜|
|Комментарии `<!-- -->` для разметки секций|⬜|
|`<hr>` (тематический разделитель)|⬜|

---

## 🔍 Шаг 5: Проверка

### В браузере

|Что проверить|Как|
|---|---|
|Страница отображается корректно|Открой через Live Server|
|Все ссылки работают|Кликни на каждую|
|Якорная навигация работает|Кликни на оглавление|
|Картинки видны|Проверь все `<img>`|
|Ссылка «Наверх» работает|Прокрути вниз и кликни|

### В DevTools

|Что проверить|Как|
|---|---|
|Структура DOM корректна|`F12` → Elements|
|Нет ошибок в Console|`F12` → Console|
|Нет 404 ошибок|`F12` → Network|

### Валидация

|Шаг|Действие|
|---|---|
|1|Открой [validator.w3.org](https://validator.w3.org/)|
|2|Выбери вкладку **«Validate by Direct Input»**|
|3|Скопируй весь HTML-код и вставь|
|4|Нажми **Check**|
|5|Исправь все ошибки (если есть)|

> [!tip] Стремись к нулю ошибок  
> Зелёное сообщение «Document checking completed. No errors or warnings to show.» — твоя цель. Это значит, что HTML написан **идеально правильно**.

---

## 📝 Задание

> [!todo] Домашнее задание
> 
> **Задание 1: Допиши статью**  
> Открой созданный файл и добавь:
> 
> - Ещё одну секцию `<h2>` на свой выбор (например, «Структура HTML-документа» или «Типы тегов»)
> - В новую секцию добавь контент, используя теги, которые ещё не использовал
> - Если не использовал `<time>`, `<var>`, `<samp>` — найди место для них
> 
> **Задание 2: Своя статья**  
> Создай **вторую статью** на любую тему (история города, обзор технологии, рассказ о хобби, описание любимой игры). Требования:
> 
> - Пройди чек-лист выше — все пункты должны быть выполнены
> - Минимум 5 секций с `<h2>`
> - Минимум 1000 символов текста
> - Оглавление с якорными ссылками
> - Проверь через W3C Validator
> 
> **Задание 3: Ревью**  
> Открой свою статью через `Ctrl + U` (исходный код) и ответь:
> 
> 1. Понятна ли структура без браузера — только по коду?
> 2. Комментарии помогают ориентироваться?
> 3. Если убрать весь текст и оставить только заголовки — получается ли логичное оглавление?
> 4. Если убрать все стили (CSS) — остаётся ли контент читаемым и структурированным?

---

## 🔑 Ключевые мысли урока

> [!abstract] Запомни
> 
> 1. **Планируй структуру** до написания кода (оглавление → заголовки → контент)
> 2. Используй **правильные теги** для каждого типа контента — это и есть семантика
> 3. **Валидируй** HTML через W3C Validator — стремись к нулю ошибок
> 4. Хорошо размеченный HTML **читаем без CSS** — структура видна из одних заголовков
> 5. **Комментарии** помогают ориентироваться в длинном файле
> 6. Правильная типографика (`&mdash;`, `&nbsp;`, `&laquo;&raquo;`) — признак профессионализма

---

## 🏁 Итог

**Поздравляю! Модуль 1 завершён!** 🎉

Ты прошёл путь от пустого файла до полноценной статьи с заголовками, абзацами, списками, ссылками, изображениями, цитатами, кодом и правильной типографикой.

Ты знаешь **более 40 HTML-тегов** и умеешь применять их на практике. Это серьёзная база, на которой строится вся дальнейшая работа.

В следующем модуле мы займёмся **таблицами** — научимся структурировать табличные данные с помощью `<table>`, `<tr>`, `<td>`, `<th>` и других тегов.

---

> [!info] Навигация  
> ← [[021 — Спецсимволы и комментарии]] | [[023 — Простая таблица]] →

