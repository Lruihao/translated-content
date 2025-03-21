---
title: Руководства по составлению документации
slug: MDN/Writing_guidelines
---

{{MDNSidebar}}

Сайт веб-документации MDN - это развивающаяся платформа для обучения Веб-технологиям и программному обеспечению, на которых основан Веб, включая:

- Веб-стандарты, например, [CSS](/ru/docs/Web/CSS), [HTML](/ru/docs/Web/HTML) и [JavaScript](/ru/docs/Web/JavaScript)
- [Разработку открытых веб-приложений](/ru/docs/Web/Progressive_web_apps)
- [Разработку дополнений Firefox](/ru/docs/Mozilla/Add-ons)

## Наша миссия

Миссия MDN очень проста: это предоставление законченной, точной и полезной документации для всего, что хоть как-то относится к [Открытому Интернету](/ru/docs/Web), и не важно является ли это программным обеспечением от Mozilla или нет. Если есть открытая технология, относящаяся к Web, мы хотим задокументировать её.

В дополнение, мы предоставляем документацию о [продуктах Mozilla](/ru/docs/Mozilla) и о том, как [разрабатывать и вносить свой вклад в проекты Mozilla](/ru/docs/Mozilla).

Если вы не уверены должна ли какая-либо тема быть представлена на MDN, прочитайте: [Нужно ли это на MDN?](/ru/docs/MDN/Writing_guidelines/What_we_write)

## Как вы можете помочь?

Вам не нужно уметь программировать или писать статьи для того, чтобы иметь возможность помочь MDN! Мы располагаем множеством вариантов того, как вы можете помочь нам, например, вы можете просматривать статьи и подтверждать, что они имеют смысл, попутно подправляя текст и добавляя примеры кода. По правде, у вас настолько много возможностей помочь нам, что мы даже подготовили специальное [руководство](/ru/docs/MDN/Community/Getting_started), которое поможет вам выбрать задачу, учитывая ваши интересы и количество времени, которое вы готовы тратить!

Также вы можете помочь, [продвигая MDN](/ru/docs/MDN/About/Promote) на вашем блоге или сайте.

## MDN сообщество

Наше сообщество глобально! В наших рядах замечательные волонтёры со всего мира, общающиеся на огромном количестве языков. Если вы хотите узнать больше или получить какую-либо помощь в MDN - присоединяйтесь к нам на [форуме обсуждений](https://discourse.mozilla-community.org/c/mdn) или [IRC-канале](irc://irc.mozilla.org#mdn)! Также вы можете следить за нашими новостями, подписавшись на наш аккаунт в Твиттере, [@MozDevNet](http://twitter.com/MozDevNet). Ещё вы можете отправлять нам твиты, если встречаетесь с какими-либо проблемами или хотите оставить свои отзывы (или поблагодарить нас) нашим создателям статей и волонтёрам!

## Использование контента MDN

### Копирайты и лицензии

**В вики-документы MDN** внесён вклад многих авторов, как внутри, так и за пределами Mozilla Foundation. Если не указано иное, содержимое доступно в соответствии с условиями [Creative Commons Attribution-ShareAlike license](https://creativecommons.org/licenses/by-sa/2.5/) (CC-BY-SA), v2.5 или более поздней версии. Пожалуйста, укажите "помощников Mozilla" и добавьте ссылку (онлайн) или URL (при печати) на вики-страницу оригинала. Например, чтобы разместить копию этой статьи, вы можете написать:

> [О MDN](/ru/docs/MDN/Writing_guidelines), создано [помощниками Mozilla](/ru/docs/MDN/About$history) и лицензируется под [CC-BY-SA 2.5](https://creativecommons.org/licenses/by-sa/2.5/).

Обратите внимание, что в этом примере ссылка "помощники Mozilla" ведёт на историю цитируемой страницы. Посмотрите [Best practices for attribution](http://wiki.creativecommons.org/Marking/Users) для дальнейшего разъяснения.

Образцы кода, добавленные в эту вики до 20 августа 2010 года, доступны под лицензией [MIT](http://www.opensource.org/licenses/mit-license.php); вы должны вставить следующую приписываемую информацию в MIT шаблон: "© <дата последней ревизии вики-страницы> <имя человека, создавшего её>".

Образцы кода, добавленные после 20 августа 2010 года являются [общественным достоянием](https://creativecommons.org/publicdomain/zero/1.0/). Наличие уведомления о лицензии не требуется, но, если вы хотите, вы можете использовать это выражение: `Any copyright is dedicated to the Public Domain. http://creativecommons.org/publicdomain/zero/1.0/`.

Если вы желаете внести свой вклад в эту вики, то вам нужно сделать свою документацию доступной по лицензии Attribution-ShareAlike (или альтернативной лицензии, указанной на странице, которую вы редактируете), и ваши образцы кода станут доступными под [Creative Commons CC-0](https://creativecommons.org/publicdomain/zero/1.0/) (и станут общественным достоянием). Добавление в эту вики означает, что вы согласны с тем, что ваш вклад будет доступен под этими лицензиями.

Некоторое более раннее содержимое было предоставлено по лицензии, отличной от указанных выше лицензий; они указаны внизу каждой страницы в виде [Alternate License Block](/Archive/Meta_docs/Examples/Alternate_License_Block).

Права на товарные знаки, логотипы, определения, принадлежащие Mozilla Foundation, а также внешний вид этого сайта, не лицензированы в соответствии с Creative Commons license, и в том виде, в котором они являются произведениями авторства (например, логотипы и графический дизайн), также они не включены в работу, которая лицензируется в соответствии с этими условиями. Если вы используете текст документов и хотите также использовать любые из этих прав, или у вас есть другие вопросы касающиеся соблюдении наших условий лицензирования для всего перечисленного, свяжитесь с Mozilla Foundation: <licensing@mozilla.org>.

### Ссылки на MDN

Мы регулярно получаем от пользователей вопросы о том, как сослаться на MDN, или даже разрешено ли это делать. Краткий ответ таков: **да, вы можете ссылаться на MDN!** Гиперссылки — это не только сама суть интернета, но и способ поделиться ценными ресурсами с вашими пользователями, продемонстрировав доверие той работе, которую делает наше сообщество.

## Скачивание контента

Вы можете скачать [полный архив содержимого MDN](https://mdn-downloads.s3-us-west-2.amazonaws.com/developer.mozilla.org.tar.gz). (2.1 ГБ, февраль 2017)

#### Отдельные страницы

Вы можете получить содержимое отдельной страницы на MDN, добавив [параметры документа](/ru/docs/MDN#document_parameters) к её URL, чтобы указать, какой формат вам нужен.

#### Сторонние инструменты

Вы можете просматривать статьи MDN с помощью сторонних инструментов, таких как [Dash](http://kapeli.com/dash) (для Mac OS) и [Zeal](http://zealdocs.org/) (для Linux и Windows).

[Kapeli](https://kapeli.com/) также публикует [онлайн-документацию MDN](https://kapeli.com/mdn_offline), содержащую HTML, CSS, JavaScript, SVG и XSLT.

## Сообщить о проблемах с MDN

Смотрите [Как сообщить о проблеме с MDN](/ru/docs/MDN/Community/Issues).

## История MDN

Сайт веб-документации MDN (ранее _Mozilla Developer Network (MDN)_, ранее _Mozilla Developer Center (MDC)_, a.k.a. _Devmo_), проект начал свою деятельность в начале 2005 года, когда [Mozilla Foundation](http://www.mozillafoundation.org) получила лицензию от AOL на использование оригинального контента Netscape [DevEdge](https://web.archive.org/web/*/devedge.netscape.com). DevEdge всё ещё создавал полезный материал, который затем был перенесён в эту вики, для того, чтобы его было легче обновлять и поддерживать.

## О Mozilla

Если хотите узнать о нас больше, где найти нас, или как стать частью _Mozilla,_ то вы попали в нужное место. Чтобы узнать, что движет нами и делает нас другими, пожалуйста, посетите страницу нашей [миссии](https://www.mozilla.org/ru/mission/).
