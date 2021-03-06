# Перевод ресурсов по Svelte

> На данный момент еще не известно в каком виде будет реализовываться внедрение локализации на официальных ресурсах, поэтому, в последствии возможны изменения в структуре и подходах данного репозитория 

## Результат нашей работы
Запущены следующие официальные русскоязычные сайты:
- [ru.svelte.dev](https://ru.svelte.dev)
- [ru.sapper.svelte.dev](https://ru.sapper.svelte.dev)
- [ru.svelte-native.technology](https://ru.svelte-native.technology)

> Сайты собираются и деплоятся автоматически при коммитах в данный репозиторий.

![](https://github.com/AlexxNB/svelte3-translation-ru/workflows/Deploy%20ru.svelte.dev%20site/badge.svg)
![](https://github.com/AlexxNB/svelte3-translation-ru/workflows/Deploy%20ru.sapper.svelte.dev%20site/badge.svg)
![](https://github.com/AlexxNB/svelte3-translation-ru/workflows/Deploy%20ru.svelte-native.dev%20site/badge.svg)

## Что переводим
* [Учебник](https://svelte.dev/tutorial) по Svelte V3 ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/content/tutorial))
* [Документацию](https://svelte.dev/docs) по Svelte V3 ([GitHub](https://github.com/sveltejs/svelte/tree/api-reference/site/content/docs))
* [Документацию](https://sapper.svelte.technology/guide) по Sapper ([GitHub](https://github.com/sveltejs/sapper.svelte.technology/tree/master/content/guide))
* [Примеры](https://svelte.dev/repl) ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/content/examples))
* [Блог](https://svelte.dev/blog) ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/content/blog))
* Контент сайта [svelte.technology](https://svelte.dev) ([GitHub](https://github.com/sveltejs/svelte/tree/master/site/src))
* Контент сайта [sapper.svelte.technology](https://sapper.svelte.technology) ([GitHub](https://github.com/sveltejs/sapper.svelte.technology/tree/master/src))
* Контент сайта [svelte-native.technology](https://svelte-native.technology) ([GitHub](https://github.com/halfnelson/svelte-native/tree/master/docs_src/content))


## Как внести свой вклад в перевод
* [Перевести](https://github.com/AlexxNB/svelte3-translation-ru/issues/6) ещё не переведённую часть какого-либо ресурса, указанного выше.
* Улучшить существующий перевод: исправить орфографическую, пунктуационную или семантическую ошибку, перефразировать неудачно скомпонованное предложение, устранить несоответствия перевода рекомендациям и т.п. Это нужно делать через систему Pull request в данном репозитории.

## Рекомендации по переводу

>Данные рекомендации по большей части подсмотрены в [сообществе переводчиков React](https://github.com/reactjs/ru.reactjs.org/blob/master/TRANSLATION.md)

* Оформление перевода должно соответствовать оформлению оригинала. 
* Где это к месту, лучше строить предложения в обезличенной форме(без `мы` и `вы`), но не фанатично, т.к. документация старается быть менее официальной. В любом случае `Вы` и его производные пишите с маленькой буквы.
* Всегда используйте букву `ё` (это соблюдать с помощью [данного npm-пакета](https://github.com/hcodes/eyo)).
* Используйте знак тире `—` — где нужно тире, и знак дефиса `-` — где нужен дефис. Примеры: как-будто, Svelte — это фреймворк.
* Во всех примерах кода необходимо переводить комментарии и весь текст, который относится к UI, т.е. то, что пользователь увидит при запуске такого примера.
* Список, с которым в порядке убывания приоритета должен быть согласован перевод лексики, терминов и прочего:
  * наш [словарь терминов](DICTIONARY.md) Svelte;
  * [словарь «Веб-стандартов»](https://github.com/web-standards-ru/dictionary);
  * аналоги в переводах документации других известных UI-фреймворков (Vue, React, Angular);
  * русскоязычная документация, доклады или статьи с использованием нужной лексики;
  * лично придуманный перевод.
* Избегать чрезмерных англицизмов, при условии, что есть общеупотребительные русские аналоги. `Пропсы`, `билд` и подобное не годятся. Но, например, `бандл` не имеет лучшего русского аналога.
* Ссылки на ресурсы (MDN, Wikipedia) должны вести на русскую версию, если есть соответствующий перевод.
* Иностранные имена переводите с указанием оригинального имени в скобках: *Рич Харрис (Rich Harris)*. При этом обязательно проверьте уже существующий перевод имени в [словаре имён «Веб-стандартов»](https://github.com/web-standards-ru/dictionary/blob/master/names.md).
* Ссылки с названием иностранной статьи в переводе должны быть приведены на языке оригинала, после чего содержать в скобках их русскоязычный перевод.
* Исключайте отсылки на пол читателя (см. секцию 3 на [этой странице](http://www.un.org/ru/gender-inclusive-language/guidelines.shtml)).
* Названия статей и заголовки пишутся с одной заглавной буквы («Удаление неиспользуемых стилей», а не «Удаление Неиспользуемых Стилей»).

Чтобы избежать кальки, можно брать смысл предложения, а потом перефразировать так, как объясняли бы старшему коллеге. Если предложение звучит нелепо вслух, то его надо переписать.

Небольшие вольности в переводе допускаются, но только если они помогают передать смысл. Перевод не должен быть ни слишком официальным, ни фамильярным. Истина где-то посередине.

## Запуск локальной версии сайта

В репозиторий добавлены npm скрипты, которые позволяют забрать с GitHub текущую версию необходимого сайта, применить все изменения из нашего репозитория переводов и запустить копию сайта на своём компьютере, чтобы сразу видеть перевод в естественных условиях.

```bash
git clone git@github.com:AlexxNB/svelte3-translation-ru.git svelte-translation
cd svelte-translation

# 1. Устанавливаем все зависимости
npm install

# 2. Скачиваем последнюю версию нужного сайта и применяем к нему перевод
npm run update-svelte 
#...или...
npm run update-sapper 
#...или...
npm run update-svelte-native 

# 3. Запускаем сайт на локальной машине
npm run dev-svelte
#...или...
npm run dev-sapper
#...или...
npm run dev-svelte-native
```

Теперь можно открыть запущенный сайт по адресу [http://localhost:3000]() и посмотреть на него со всеми внесёнными изменениями на текущий момент.

При изменении файлов перевода, обновите окно браузера и вы должны будете увидеть изменения.
