---
title: <main>
slug: Web/HTML/Reference/Elements/main
---

{{HTMLSidebar}}

HTML-элемент **`<main>`** представляет основное содержимое {{HTMLElement("body", "тела")}} документа. Эта область должна состоять из содержимого, которое напрямую связано с центральной темой документа или с основными функциями приложения.

{{InteractiveExample("HTML Demo: &lt;main&gt;", "tabbed-shorter")}}

```html interactive-example
<header>Gecko facts</header>

<main>
  <p>
    Geckos are a group of usually small, usually nocturnal lizards. They are
    found on every continent except Antarctica.
  </p>

  <p>
    Many species of gecko have adhesive toe pads which enable them to climb
    walls and even windows.
  </p>
</main>
```

```css interactive-example
header {
  font:
    bold 7vw Arial,
    sans-serif;
}
```

Документ не должен иметь более одного элемента `<main>` у которого не указан атрибут [`hidden`](/ru/docs/Web/HTML/Reference/Global_attributes#hidden).

| [Категории контента](/ru/docs/Web/HTML/Guides/Content_categories) | [Основной поток](/ru/docs/Web/HTML/Guides/Content_categories#основной_поток), [явный контент](/ru/docs/Web/HTML/Guides/Content_categories#явный_контент).                                                                                                                                               |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Допустимое содержимое                                             | [Основной поток](/ru/docs/Web/HTML/Guides/Content_categories#основной_поток).                                                                                                                                                                                                                           |
| Пропуск тегов                                                     | Ни одного; Оба тега, открывающий и закрывающий, являются обязательными.                                                                                                                                                                                                                                 |
| Допустимые родители                                               | Те, в которых разрешается [контент основного потока](/ru/docs/Web/HTML/Guides/Content_categories#основной_поток) в качестве содержимого, но только если это [иерархически корректный `main` элемент](https://html.spec.whatwg.org/multipage/grouping-content.html#hierarchically-correct-main-element). |
| Допустимые ARIA-роли                                              | Роль `main` применяется к `<main>` по умолчанию, и роль [`presentation`](/ru/docs/Web/Accessibility/ARIA/Roles/presentation_role) также разрешена.                                                                                                                                                      |
| DOM-интерфейс                                                     | {{domxref("HTMLElement")}}                                                                                                                                                                                                                                                                              |

## Атрибуты

К этому элементу применимы только [глобальные атрибуты](/ru/docs/Web/HTML/%D0%9E%D0%B1%D1%89%D0%B8%D0%B5_%D0%B0%D1%82%D1%80%D0%B8%D0%B1%D1%83%D1%82%D1%8B).

## Примечание

Содержимое элемента `<main>` должно быть уникальным для документа. Содержимое, которое повторяется в наборе документов или разделах документа, такое как боковые панели, навигационные ссылки, информация об авторских правах, логотипы сайта и поисковые формы, не должно добавляться, за исключением формы поиска, если она является основной функцией страницы.

`<main>` не вносит вклад в структуру документа; то есть, в отличие от таких элементов, как {{HTMLElement("body")}}, заголовков, таких как {{HTMLElement("h2")}} и т.п., `<main>` не влияет на концепцию {{glossary("DOM")}} структуры страницы. Он носит исключительно информативный характер.

## Пример

```html
<!-- другой контент -->

<main>
  <h1>Яблоки</h1>
  <p>Яблоко - плод яблони, который употребляется в пищу в свежем виде, служит сырьём в кулинарии и для приготовления напитков.</p>

  <article>
    <h2>Сорт "Ред Делишес"</h2>
    <p>Эти ярко-красные яблоки являются одними из самых популярных в Соединённых Штатах.</p>
    <p>... </p>
    <p>... </p>
  </article>

  <article>
    <h2>Сорт "Гренни Смит";/h2>
    <p>Эти сочные, зелёные яблоки являются одними из самых популярных в мире.</p>
    <p>... </p>
    <p>... </p>
  </article>
</main>

<!-- другой контент -->
```

### Результат

{{EmbedLiveSample("Пример")}}

## Доступность

### Ориентир

Элемент `<main>` ведёт себя как [роль-ориентир `main`](/ru/docs/Web/Accessibility/ARIA/Roles/Main_role). [Ориентиры](/ru/docs/Web/Accessibility/ARIA/Guides/Techniques#landmark_roles) могут использоваться вспомогательными технологиями для быстрой идентификации и навигации по большим разделам документа. Предпочтительно использовать элемент `<main>` вместо объявления `role="main"`, если не нужна [поддержка старых браузеров](/ru/docs/Web/HTML/Reference/Elements/main#%D0%9F%D0%BE%D0%B4%D0%B4%D0%B5%D1%80%D0%B6%D0%BA%D0%B0_%D0%B1%D1%80%D0%B0%D1%83%D0%B7%D0%B5%D1%80%D0%B0%D0%BC%D0%B8).

### Пропуск навигации

Пропуск навигации, также известный как "skipnav", это техника которая позволяет пользователю вспомогательных технологий совершать быстрый обход больших разделов повторяющегося контента (главная навигация, информационные баннеры и т.д.). Это позволяет пользователю получить доступ к основному контенту страницы быстрее.

Добавление атрибута [`id`](/ru/docs/Web/HTML/Reference/Global_attributes#id) в элемент `<main>` позволяет ему становится целью для ссылки пропуска навигации.

```html
<body>
  <a href="#main-content">Перейти к основному контенту</a>

  <!-- навигация и заголовок контента -->

  <main id="main-content">
    <!-- основной контент страницы -->
  </main>
</body>
```

- [WebAIM: Ссылки "Пропуск навигации"](https://webaim.org/techniques/skipnav/)

### Режим чтения

Функционально режим чтения браузера будет искать наличие элемента `<main>`, а также элементов [заголовка](/ru/docs/Web/HTML/Reference/Elements/Heading_Elements) и [секционных элементов](/ru/docs/Web/HTML/Reference/Elements#%D0%A1%D0%B5%D0%BA%D1%86%D0%B8%D0%BE%D0%BD%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5_%D1%81%D0%BE%D0%B4%D0%B5%D1%80%D0%B6%D0%B0%D0%BD%D0%B8%D1%8F), которые преобразовывают контент в специальный вид для чтения.

- [Создание сайтов для режима чтения Safari и других программ чтения.](https://medium.com/@mandy.michael/building-websites-for-safari-reader-mode-and-other-reading-apps-1562913c86c9)

## Спецификации

{{Specifications}}

## Совместимость с браузерами

Элемент `<main>` широко поддерживается. Для Internet Explorer 11 и ниже предлагается добавить роль {{glossary("ARIA")}} `"main"` в элемент `<main>`, чтобы обеспечит его доступность (программы для чтения с экрана, такие как JAWS, используемые совместно со старыми версиями Internet Explorer, смогут понять семантическое значение элемента `<main>` после добавления атрибута `role`).

```html
<main role="main">...</main>
```

{{Compat}}

## Смотрите также

- Основные структурные элементы: {{HTMLElement("html")}}, {{HTMLElement("head")}}, {{HTMLElement("body")}}
- Связанные с этим разделом элементы: {{HTMLElement("article")}}, {{HTMLElement("aside")}}, {{HTMLElement("footer")}}, {{HTMLElement("header")}}, or {{HTMLElement("nav")}}
- [ARIA: роль main](/ru/docs/Web/Accessibility/ARIA/Roles/Main_role)
