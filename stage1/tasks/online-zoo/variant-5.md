# Вариант #5

Выполнить задание согласно макету автора *Noora Sagnayeva*: **[zooApp](https://www.figma.com/file/HKt5Nlx0jghQtJp6jW9q8F/zooApp)**


## Создание макета: неделя #1+2

Выполняется создание всех страниц для ширины экрана **1920px**.


### Технические требования

Максимальный балл: **80**


#### Общие

Все фоновые элементы макета должны растягиваться на всю доступную ширину экрана, если ширина больше 1920px. При этом направляющие должны сохраняться в исходном размере, 1400px. Особенностью этого проекта является поддержка двух цветовых тем. Важно, что ни в коем случае, на странице не должна появляться горизонтальная полоса прокрутки. О таких случаях будет сказано в технических требованиях соотвествующих блоков.

Для создания вертикальных отступов лучше использовать вертикальные margin на блоках высшего порядка, насколько это возможно. При этом иметь ввиду, что вертикальные margin могут схлопнуться.

Для создания многоколоночных структур, или элементов имеющих относительное горизонтальное расположение, должно быть использовано одно из свойств:
- display: flex
- display: grid
- display: inline-block


#### Landing (30 баллов)

1. **Header** (`<header>` содержит только логотип, панель навигации и кнопку смены темы)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на текущую страницу, на First Page. Landing.
- Интерактивная панель навигации.
- (5) Должен быть подсвечен первый элемент `About`. И он должен перестать быть интерактивным.
- Нажатие на `Map` перебрасывает нас на intermediatePage.
- Нажатие на `Zoos` перебрасывает нас на LIVE_BROADCAST с пандой.
- Нажатие на `Contact Us` перебрасывает нас вниз страницы на форму обратной связи.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/HKt5Nlx0jghQtJp6jW9q8F/zooApp).
- Интерактивный переключатель цветовой темы.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. Блок **Watch your favorite animal online**
- (5) Задний фон является картинкой.
- Кнопка `Watch online` должна быть интерактивной.
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.
- Картинки животных должны быть интерактивными. Нажатие на кнопку `watch online` перебрасывает нас на LIVE_BROADCAST соотвествующего животного.
- Полоска прогресса должна быть интерактивной. Начинаем со значания `02 / 08`.

3. Блок **How it works**
- Полоска прогресса должна быть интерактивной. Начинаем со значания `01 / 04`.
- Кнопка `Watch online` должна быть интерактивной.

4. Блок **What's inspiring us?**
- (5) Трехколоночный макет.

5. Блок **Pets in zoo**
- Кнопки влево и вправо должны быть интерактивными. При нажатии ничего происходить не должно.
- Карточки животных должны быть интерактивными. При наведении курсора должна быть анимация выезда текста снизу картинки. Сама картинка при этом должна затемниться.
- Кнопка `Choose your favorite` должна быть интерактивной. При нажатии ведет нас на страницу `Map`.
- Полоска прогресса должна быть интерактивной. Начинаем со значания `01 / 08`.

6. Блок **Pay and feed**
- Кнопка `Donate` должна быть интерактивной. При нажатии ничего происходить не должно.

7. Блок **Testimonials**
- Кнопки влево и вправо должны быть интерактивными. При нажатии ничего происходить не должно.
- Полоска прогресса должна быть интерактивной. Начинаем со значания `01 / 08`.
- Кнопка `Leave feedback` должна быть интерактивной.

8. Блок **Map**
- (5) На карте должно быть 4 интерактивных иконки. При наведении должна быть анимация, когда элемент меняет цвет. Также, при наведении должно появляться окно-подсказка, и этот процесс можно реализовать средствами CSS. Точка, где всплывает подсказка - не имеет значения, главное чтобы этот блок не выходил за край экрана. При нажатии может ничего не происходить.
- (5) Кнопка `Watch online` должна перебрасывать нас на LIVE_BROADCAST с выбранным животным. На данном этапе, нас перебрасывает на LIVE_BROADCAST с пандой.

9. **Footer** (`<footer>` содержит меню, доготипы, кнопки доната и соц. сетей):
- Нажатие на логотип работает по принципу нажатия на About, перебрасывает нас на верх текущей страницы, на Landing.
- В блоке `Contact Us` находится форма. Все поля, включая чекбокс, должны быть обязательными для заполнения.
- Name - поле `input` с типом `text`.
- Email - поле `input` с типом `email`.
- (5) Please enter your message - поле `textarea` c ограничением в 280 символов. Для обрамления используйте `fieldset` и `legend`.
- I agree to ... - поле `input` с типом `checkbox` и `label`.
- Текст `send` и картинка стрелки - это все одна кнопка с типом `submit`
- (5) Нажатие на `About` перебрасывает нас на верх страницы. Просто ссылка на эту же страницу.
- Нажатие на `Map` перебрасывает нас на intermediatePage.
- Нажатие на `Zoos` перебрасывает нас на LIVE_BROADCAST с пандой.
- Кнопка `Donate for volunteers` должна быть интерактивной.
- Под заголовком `ZOO Online Centre` располагается тег address, в котором в свою очередь должны располагаться правильно указанные ссылки на почту `mailto` и на телефон `tel`. Обратите внимание, что буква `T` не является частью номера телефона.


#### Map (10 баллов)

1. **Header** (`<header>` содержит только логотип, панель навигации и кнопку смены темы)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на текущую страницу, на First Page. Landing.
- Интерактивная панель навигации.
- Нажатие на `About` перебрасывает нас на DESKTOP (Landing).
- (5) Должен быть подсвечен элемент `Map`. И он должен перестать быть интерактивным.
- Нажатие на `Zoos` перебрасывает нас на LIVE_BROADCAST с пандой.
- Нажатие на `Contact Us` перебрасывает нас вниз страницы на форму обратной связи.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/HKt5Nlx0jghQtJp6jW9q8F/zooApp).
- Интерактивный переключатель цветовой темы.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. Блок **Map**
- Кнопки влево и вправо должны быть интерактивными. При нажатии ничего происходить не должно.
- Иконки животных в карусели должны быть интерактивными. Должен быть выбран второй элемент в списке - панда. При нажатии ничего происходить не должно.
- (5) На карте должно быть 4 интерактивных иконки. Должна быть подсвечена иконка панды. При нажатии ничего происходить не должно. При наведении должен появляться базовый тултип с подсказкой - название животного, сделанный через аттрибут `title`.
- (5) Кнопка `Watch online` должна перебрасывать нас на LIVE_BROADCAST с выбранным животным. На данном этапе, нас перебрасывает на LIVE_BROADCAST с пандой.

3. **Footer** (`<footer>` содержит меню, доготипы, кнопки доната и соц. сетей):
- Интерактивная панель навигации. По умолчанию, элементы не имеют подсветки.
- Нажатие на `About` перебрасывает нас на First Page. Landing.
- Нажатие на `Map` перебрасывает нас на Map Page.
- Нажатие на `Contact Us` перебрасывает нас на Contact Us.
- Кнопка `Donate for volunteers` должна быть интерактивной.
- Логотипы не интерактивные. Они не должны реагировать на нажатие. Но должен появлятся тултип (атрибут title) с соотвествующей надписью (Online Zoo, Yem Digital, Rolling Scopes School).
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.

#### Zoos page (10 x 4 = 40 баллов)
Требования для типовой страницы. Переход осуществляется по ссылкам типа `.../zoos/panda` или `.../zoos/alligator`

1. **Header** (`<header>` содержит только логотип, панель навигации и кнопку смены темы)
- Логотип находится слева. Нажатие на логотип работает по принципу нажатия на `About`, перебрасывает нас на текущую страницу, на First Page. Landing.
- Интерактивная панель навигации.
- Нажатие на `About` перебрасывает нас на DESKTOP (Landing).
- Нажатие на `Map` перебрасывает нас на intermediatePage.
- (5) Должен быть подсвечен элемент `Zoos`. И он должен перестать быть интерактивным.
- Нажатие на `Contact Us` перебрасывает нас вниз страницы на форму обратной связи.
- Нажатие на `Design` перебрасывает нас на оригинальную страницу [Figma](https://www.figma.com/file/HKt5Nlx0jghQtJp6jW9q8F/zooApp).
- Интерактивный переключатель цветовой темы.
- На странице обязательно должен присутствовать один элемент `<h1>`. В нем должен быть текст `Online Zoo`.
- Хедер "липким" делать не нужно. Т.е. при скролле он остается на своей позиции.

2. **Side bar** (`<aside>`)
- Панель слева: Должно быть подсвечено выбранное животное.
- Панель слева: При скролле, как только экран опускается ниже хедера, меню с животными должно "прилипнуть" к боковой части экрана. На этот счет ознакомьтесь с [position: sticky](https://css-tricks.com/creating-sliding-effects-using-sticky-positioning/). И опускаться ровно до футера, где эффект потреяет силу.
- При наведении на иконку животного должен появится тултип с названием животного, можно офромить в виде атрибута `title`.
- Выбранное животное становится не интерактивным, но тултип должен остаться.

3. Блок **The Zoo**
- Блок видео - это элемент `iframe` с видео трансляции, его можно добавить на страницу по [инструкции](https://support.google.com/youtube/answer/171780?hl=ru).
- Кнопка `Feed` должна быть интерактивной.
- Картинки в карусели - это должны быть либо превью с youtube, либо такие же `iframe` с видео. Сверху самих видео надо наложить полностью прозрачный элемент, который не даст нажать видео, и ничего не произойдет. Эта заглушка нужна будет при работе с js.
- Кнопки под слайдером должны быть интерактивными. При нажатии ничего происходить не должно.
  
4. **Footer** (`<footer>` содержит меню, доготипы, кнопки доната и соц. сетей):
- Интерактивная панель навигации. По умолчанию, элементы не имеют подсветки.
- Нажатие на `About` перебрасывает нас на First Page. Landing.
- Нажатие на `Map` перебрасывает нас на Map Page.
- Нажатие на `Contact Us` перебрасывает нас на Contact Us.
- Кнопка `Donate for volunteers` должна быть интерактивной.
- Логотипы не интерактивные. Они не должны реагировать на нажатие. Но должен появлятся тултип (атрибут title) с соотвествующей надписью (Online Zoo, Yem Digital, Rolling Scopes School).
- Интерактивная панель соцсетей. Нажатия на соцсети могут вести просто на заглавные страницы соотвествующих ресурсов.


## Адаптивность: неделя #3

Сверстанные страницы адаптируюятся под следующую ширину экрана устройства:
- 1920px (уже будет готово)
- 1200px
- 640px
- 320px

### Технические требования

Максимальный балл: **40**

🚧 Задание в процессе разработки 🚧


## Функционалная часть и пользовательские события: неделя #4-5

Добавление JavaScript.

### Технические требования

Максимальный балл: **80**

🚧 Задание в процессе разработки 🚧