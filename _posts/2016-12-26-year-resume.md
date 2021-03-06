---
layout:     post
title:      Итоги 2016 года от CSSSR
---

Всем привет! Меня зовут Максим, и я работаю верстальщиком в CSSSR.

Сегодня мы решили вспомнить события и людей уходящего года, поделиться, чем он нас порадовал или огорчил, какие ожидания оправдал, а какие — нет. Одним словом, сегодня подведём итоги 2016-го.

## Релиз TypeScript 2.0–2.1

![image](/images/year-resume/typescript.png)

Часто сталкивались с `undefined is not a function`? Или интернет магазин начислил вам `NaN бонусов`? А как насчет такси, которое приедет через `null минут`? Слабая динамическая типизация уже давно является ахиллесовой пятой JS. А недавно мы на самих себе прочувствовали всю боль отсутствия статической типизации в проекте из 4-х(!) языков программирования. В общем, фронтенд получил полноценное оружие объявления типов, что не может не радовать.

## Сборка фронтенда в 2016-м

![image](/images/year-resume/webpack.jpg)

Ребус на картинке выше — это технологии, из которых можно сложить следующее предложение: `«Webpack в 2016-м году»`.

Казалось бы, как Webpack мог стать популярным, будучи технологией, крайне недружелюбной в основении и требующей зачастую сил отдельного специалиста? 1–1,5 года назад все проблемы по сборке и автоматизации решались простой командой `npm i -g gulp`. Сегодня же стремительно вырисовывается гегемония Webpack'a, для которого в 2016 году сформировался полный набор плагинов, позволяющий полноценно собирать проекты.

Сборка стала еще быстрее! Еще!

## Сборка фронтенда в 201*-м

Есть ли в вашей жизни место мистике? Верите ли вы в жизнь после смерти? Если да, то теперь вы стали еще на шаг ближе к просветлению. А если нет, то сейчас мы докажем существования загробной жизни.

![image](/images/year-resume/grunt.png)

[21.09.2011 - 4.04.2016](https://twitter.com/gruntjs/status/717134434357501952)

Продукт релизнулся спустя два года после своей смерти! Этот твит, как ничто другое, показывает текущую скорость развития фронтенда.

## Установка зависимостей в 2016-м

![image](/images/year-resume/yarn.png)

Казалось, что правление npm будет вечным, однако новорожденный [Yarn](https://yarnpkg.com/) поразил всех не только своей скоростью, но и вменяемым контролем версий, чем стремительно заявил о своих правах на престол установки пакетов.

Npm умер! Да здравствует Yarn.

## ФП в JS

![image](/images/year-resume/fp.png)

Есть языки настолько высокоуровневые, что вы легко начнёте программировать в концепциях, которые исключают все известные паттерны программирования. Это фунциональные языки.

В 2016 году каждый фронтенд-программист убежден в своем священном долге изучать и применять постулаты Алонсо Чёрча в повседневной работе. Использование монад, чистых функций, каррирования — не это ли знакомые заголовки. Ни одна JS-конференция в этом году не обошла стороной использование функциональной парадигмы в веб-разработке.

Пока что сложно сказать о неизбежно скором переходе к функциональным языкам, но первые сигналы уже прозвучали: Elm, ClojureScript, ramda. Умы разработчиков поглощены философией математики, понятиями которой оперируют функциональные языки, и кто знает к чему это приведет? Однажды мир веб-разработки уже потряс результат увлечения Elm'ом, и мы получили Redux.

### The Return of Stream I/O

![image](/images/year-resume/stream.png)

Позвольте нам немного старческого брюзжания. Новое — это хорошо забытое старое, и JavaScript не стал исключением. Сегодня многие разработчики используют Redux, но при этом не знают, на каких идеях он стоит. Эти идеи идут далеко за пределы Elm, прямиком в 1970-e года, когда были разработаны первые языки, в которых разные участки кода общались между собой при помощи [обмена сообщениями](https://ru.wikipedia.org/wiki/%D0%9E%D0%B1%D0%BC%D0%B5%D0%BD_%D1%81%D0%BE%D0%BE%D0%B1%D1%89%D0%B5%D0%BD%D0%B8%D1%8F%D0%BC%D0%B8). В 90-х Java и другие ООП языки второй волны отказались от «обмена сообщениями», предоставив взамен концепцию «вызова метода».

Однако время все раставило по своим местам. На концепции «обмена сообщениями» сегодня так или иначе основаны почти все фронтенд инструменты: знакомый Redux, маргинальные Elm и Cycle.js, весьма популярные Observable/Stream (Angular 2) и computed (MobX, Vue.js, Ember.js и многие другие).

Это произошло, потому что выросли требования к интерактивности веб-приложений. Осенью 2016 [Andre Medeiros](http://staltz.com/) выступил с [докладом](https://www.youtube.com/watch?v=Tkjg179M-Nc), в котором рассказал о том, почему мы вдруг вернулись к столь старым идеям во фронтенде, почему это хорошо и какие у них перспективы.

## Укрепление Redux как общепонятного стандарта при работе с React'ом (и не только)

Быстрый переход в начале года от Flux-архитектуры породил волну непонимания — а как вообще тогда работать с React'ом? Предлагалось использование immutable.js и его дополнительного интерфейса, поэтому многие конторы пилили собственные велосипеды. В итоге мы получили один стор, чистые функции, бойлерплейт для сложных кейсов <s>и стрелять по ногам стало ещё сложнее</s>. Структура бойлерплейтов React-проектов стала более менее похожа, и в её сердце практически всегда Redux.

## Project Tofino

![image](/images/year-resume/ff.png)

Команда Mozilla начала разработку [гибридного браузера](https://github.com/mozilla/tofino), которой должен стать новой вехой во взаимодействии пользователя и интерфейса.

Еще более интересен тот факт, что внутрь Tofino встроена база данных [Datomish](https://medium.com/project-tofino/introducing-datomish-a-flexible-embedded-knowledge-store-1d7976bff344#.3exien4py), основанная на идеях логического программирования и CQRS. Возможно, в недалеком будущем вместо довольно примитивных localStorage и IndexedDB мы получим полноценное графовое хранилище в браузере с мощным языком запросов и возможностью синхронизации между различными устройствами.

Так или иначе, но тот Firefox, который мы знаем, возможно скоро перестанет существовать.

## Скандал с left-pad

23 марта [Азер Кочулу](https://medium.com/@azerbike/i-ve-just-liberated-my-modules-9045c06be67c#.2t9nzr5aa) показал всему миру, как что-то вроде бы небольшое и незначительное может повлиять на жизни тысяч людей, особенно если речь идет об npm-пакете. «Что? Какой left-pad? Я устанавливал Node/Babel/React!». В тот день казалось, что обращениям в ишью не будет конца, а при установке падал практически любой npm-пакет. Тогда интернет остановился на несколько часов.

Конечно, все разрешилось, и теперь разработчики всего мира знают: любой пакет, если что, [npm может вернуть](https://twitter.com/seldo/status/712414588281552900). Даже несмотря на мнение автора.

Инцидент с left-pad обнажил один из самых страшных пороков веб-разработки: отсутствие четкой стандартизации и регламентации при разработке и распространении ПО. Каждый может повлиять на каждого.

## Сетка

![image](/images/year-resume/grid.png)

Этот год был богат на события не только в мире JavaScript, но и в мире CSS.

[Спецификация Grid Layout](https://www.w3.org/TR/css-grid-1/) получила статус кандидата в рекомендации, что, несоменно, стало отдушиной для всех верстальщиков. Grid Layout и FLexbox, очевидно, станет последним гвоздем в крышку гроба, где покоятся флоаты и инлайн-блоки.

## CSSSR в 2016

Год был богат не только на общемировые события, но и на наши внутрикорпоративные.

#### Релиз HR-tools

У нас появился не только инструмент для сбора заявок от кандидатов, но и полноценная база данных, позволяющая просматривать, оценивать и комментировать тестовые задания от соискателей.

![image](/images/year-resume/hr1.png)

Оценка проводится в два этапа — оценка тестового задания и оценка собеседований.

![image](/images/year-resume/hr2.png)

Заинтересованы? [Го к нам, уже создали](http://csssr.ru/jobs#).

#### [#react-learning-club](https://www.youtube.com/user/John1744444/videos)

![image](/images/year-resume/rlc.png)

С ростом штата компании остро стал вопрос о централизованном повышении квалификации сотрудников. С этой целью был предложен локальный проект, где начинающие разработчики могли бы попробовать свои сиды в написании фронтенд- или fulltack-приложений. Однако, проект быстро разросся и превратился в настоящий испытательный полигон для разработчиков самого разного уровня. Часть уроков построена в формате парного программирования (ученик — гуру), и таким образом обучаемый получает моментальный фидбек по своим действиям.

Ссылка на записи заседаний клуба вынесена в заглавие, подписывайтесь на канал, ставьте лайки.

#### [blog.csssr.ru](http://blog.csssr.ru)

В этом году наше присутствие на интернет-арене необычайно усилилось. Наши статьи попали во все крупные интеренет-издания и паблики, породив тонны холиваров <s>и срачей</s>:

- [Web-Standards](https://twitter.com/webstandards_ru/status/778217300163956736)
- [Еще Web-Standards, пруфы с 26.50](https://soundcloud.com/web-standards/episode-46)
- [Еще Web-Standards](https://twitter.com/webstandards_ru/status/807175305798553600)
- [Еженедельный дайджест от Habrahabr](https://habrahabr.ru/company/zfort/blog/310980/)
- [Еще статья на Habrahabr](https://habrahabr.ru/post/312932/)
- [Medium](https://medium.com/russian/%D0%BF%D0%BE%D0%BB%D0%B5%D0%B7%D0%BD%D1%8B%D0%B5-%D0%BF%D1%80%D0%B8%D0%B2%D1%8B%D1%87%D0%BA%D0%B8-%D0%B4%D0%BB%D1%8F-%D1%83%D0%B4%D0%B0%D0%BB%D1%91%D0%BD%D0%BD%D0%BE%D0%B9-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B-edd8926deab1#.uxdtvqho0)
- [TomskJS](https://vk.com/tomskjs?z=video-96860508_456239017%2F32af932478766965c3%2Fpl_wall_-96860508)
- [CodeFest](https://www.youtube.com/watch?v=2oh0EeJrBVY)

## Послесловие
А, ну еще Angular 2 релизнулся, но об этом, видимо в следующем году.


