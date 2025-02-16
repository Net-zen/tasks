| Deadline | Folder name | Branch name |
| ----------- | ------------- | ------------- |
| 15.12.2019 23:59 | fancy-weather | fancy-weather |

# fancy-weather

## Задание

Вам необходимо создать приложение - прогноз погоды

### Структура приложения

Приложение состоит из четырёх функциональных блоков.

**Блок 1. Блок контроля**

- кнопка для переключения фонового изображения
- кнопка для переключения языка (en/ru/be)
- кнопка для переключения единиц измерения температуры (°C/°F)
- строка поиска

**Блок 2. Погода за сегодня**

- название населённого пункта, название страны
- текущая дата: день недели в коротком формате, число, месяц, например, Сб 26 октября
- время: часы и минуты, например, 17:23, обновляется раз в минуту
- температура в текущий промежуток времени
- описание погоды (summary), ощущаемая температура (apparent temperature), скорость ветра(м/с), влажность(%)
- иконка погоды

**Блок 3. Прогноз погоды на три дня**

- день недели в полном формате
- средняя температура
- иконка погоды

**Блок 4. Геолокационные данные**

- координаты населённого пункта: долгота и широта (в градусах и минутах)
- карта местности

Дизайн приложения на ваше усмотрение.  
Один из возможных вариантов оформления приложения: [Макет в Figma](https://www.figma.com/file/3aQwTNcZWg5CTuvlQ1t5MQ/fancy-weather?node-id=0%3A1)

## Требования к функционалу приложения

- Когда пользователь открывает приложение, все данные на странице относятся к текущему местоположению пользователя
- В строке поиска осуществляется поиск по населённому пункту
- Фоновое изображение изменяется при обновлении страницы или при клике по кнопке для переключения фонового изображения в блоке контроля
  - фоновые изображения генерируются с учётом поры года, времени суток, текущей погоды, страны, названия населённого пункта
- Настройки при первом запуске приложения: язык – английский, единицы измерения температуры – градусы Цельсия: 
  - переключатель языка изменяет язык отображения текста страницы (en/ru/be).  
  - переключатель температуры изменяет единицы измерения температуры (°C/°F).
  - пользовательские настройки языка и температуры сохраняются в local storage.

## Оценивание

**Максимальный бал за задание: 280**

### Базовый уровень

- верстка прототипа приложения адаптивная или респонсив – **20 баллов**
  - минимальная ширина страницы, при которой она отображается корректно – 320 рх
- В блоке 2 отображаются данные, относящиеся к текущему местоположению пользователя – **20 баллов**
- В блоке 3 отображается прогноз погоды на три дня, относящийся к текущему местоположению пользователя – **20 баллов**
- В блоке 4 отображаются геолокационные данные, относящиеся к текущему местоположению пользователя (широта, долгота, карта) – **20 баллов**  
  **Всего 80 баллов**

### Средний уровень

- Реализован поиск. Если в поиске вводится корректный запрос, все данные на странице, в том числе дата и время, обновляются в соответствии с указанным в поиске населённым пунктом – **60 баллов**
- При обновлении страницы или клике на кнопку для переключения фонового изображения меняется фоновое изображение – **20 баллов**
- Реализована возможность переключения единиц измерения температуры – **10 баллов**
- Выполнены требования к коду – **30 баллов**
  - html-элементы генерируются в js
  - js код разбит на модули
  - используется webpack
  - используются editorconfig, eslint, eslint-config-airbnb-base, babel  
    **Всего 120 баллов**

### Экстра-уровень

- Реализована возможность голосового поиска по названию населённого пункта – **20 баллов**
- Реализованы юнит-тесты – 2 балла за каждый тест, но не больше **20 баллов**
- Реализован перевод текста страницы (en/ru/be) – **20 баллов**
- Бонусные баллы за качество приложения – **20 баллов**
  - кнопки, иконки приложения анимированы, для анимации использованы ключевые кадры
  - в дизайне приложения продуманы и реализованы кастомные уникальные элементы и/или в приложении продуман и реализован не предусмотренный заданием дополнительный функционал  
    **Всего 80 баллов**

### Штрафные баллы

- ошибки в консоли на любом этапе работы приложения – **10 баллов**
- использование вместо собственных ключей доступа к API ключей, указанных в описании задания – **10 баллов**
- меньше 6 коммитов, ошибки в названиях коммитов, ошибки в оформлении пулл реквеста – **10 баллов**  
  **Всего 30 баллов**

## Технические требования

- приложение корректно работает в последней версии Chrome
- можно использовать css-препроцессоры, bootstrap, material design, lodash.js
- использование jQuery и других js-библиотек не допускается
- запрещено использование Angular / React / Vue

### Ключевые навыки

- работа с API
- получение данных при помощи асинхронных запросов

<details> 
  <summary>Материалы</summary>
  
- **Документ с вопросами и ответами**
  - https://docs.google.com/spreadsheets/d/18BviVQSPjlrkByibrf7dg1ZXhNID66PBhrblXyNMFy8/edit#gid=0
- **Асинхронные запросы, fetch/async/await**
  - [Асинхронные запросы. Использование Fetch](https://developer.mozilla.org/ru/docs/Web/API/Fetch_API/Using_Fetch)
  - [Асинхронные функции (async/await)](https://youtu.be/5kAPExqSZ1I)
  - [JavaScript Fetch API and using Async/Await](https://dev.to/shoupn/javascript-fetch-api-and-using-asyncawait-47mp)

- **Дата и время**
  - [Date](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Date)
  - [Date.prototype.toLocaleString](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Date/toLocaleString)

- **Распознавание голоса в браузере**
  - [SpeechRecognition](https://developer.mozilla.org/ru/docs/Web/API/SpeechRecognition)
  - [JavaScript Speech Recognition](https://www.youtube.com/watch?v=0mJC0A72Fnw)

- **API погоды**
  - [React-приложение Прогноз погоды на 5 дней](https://medium.com/@leizl.samano/how-to-make-a-weather-app-using-react-403c88252deb)
  - [React-приложение Прогноз погоды](https://tproger.ru/translations/react-basic-weather-app/)

- **Советы по качеству кода**
  - [Магические числа](https://ru.code-basics.com/languages/javascript/modules/variables/lessons/magic-numbers)
  - [Как писать чистый код: обзор лучших практик JavaScript](https://techrocks.ru/2019/08/27/writing-clean-code-in-javascript/)
  - [Рекомендации по написанию чистого кода на JavaScript](https://habr.com/ru/company/ruvds/blog/454520/)
</details>

<details> 
  <summary>API с примерами подключения</summary>
  
**1. Данные о текущем местоположении пользователя**    
- https://ipinfo.io/ 
  - регистрируемся на сайте
  - получаем токен 
  - получаем данные о местоположении пользователя  
  `https://ipinfo.io/json?token=eb5b90bb77d46a` 
  - [API Docs](https://ipinfo.io/developers)

**2. API погоды**  
OpenWeatherMap, Weatherbit, AccuWeather, Dark Sky, Weather2020 и др.

- https://openweathermap.org/
  - регистрируемся на сайте
  - получаем API Key  
    `https://home.openweathermap.org/api_keys`
  - получаем данные о погоде на ближайшие пять дней  
    `https://api.openweathermap.org/data/2.5/forecast?q=Kiev&lang=ua&units=metric&APPID=a9a3a62789de80865407c0452e9d1c27`
  - [API Docs](https://openweathermap.org/api)
- https://darksky.net/
  - регистрируемся на сайте
    `https://darksky.net/dev/register`
  - подтверждаем email (переходим по ссылке, которая пришла на почту)
  - получаем Secret Key
  - получаем данные о погоде погоде на ближайшие семь дней  
    `https://api.darksky.net/forecast/2bf27985f5a6844febcdc43c99cc81ce/53.5359,27.3400?lang=be`
  - [API Docs](https://darksky.net/dev/docs)

**3. Фото для фона**

- https://unsplash.com/developers
  - регистрируемся на сайте
  - подтверждаем email (переходим по ссылке, которая пришла на почту)
  - создаём приложение  
    `https://unsplash.com/oauth/applications`
  - получаем Access Key
  - получаем фото для фона, которое меняется при каждом обновлении страницы  
    `https://api.unsplash.com/photos/random?orientation=landscape&per_page=1&query=nature&client_id=e2077ad31a806c894c460aec8f81bc2af4d09c4f8104ae3177bb809faf0eac17`
  - у данного сервиса есть лимит - 50 изображений в час
  - [API Docs](https://unsplash.com/documentation)
- https://www.flickr.com/services/
    - регистрируемся на сайте
    - подтверждаем email (переходим по ссылке, которая пришла на почту)
    - создаём приложение `https://www.flickr.com/services/apps/create/apply/`
    - получаем API Key
    - [API Docs](https://www.flickr.com/services/api/)
    - [The Flickr
Developer Guide](https://www.flickr.com/services/developer/api/)
    - Still have questions? Check out [code.flickr.com](https://code.flickr.net/) or the [FAQs](https://help.flickr.com/)!
    - демонстрационный пример работы с API Flickr [demo](https://flickr-api-test.netlify.com/)
    _Внимание_ у Flickr огромный и не всегда очевидный в работе api, выбирая Flickr, будьте осторожны и терпеливы

**4. Геолокакция**

- [Geolocation API](https://developer.mozilla.org/ru/docs/Web/API/Geolocation/getCurrentPosition)

**5. Картографические API**  
Google Maps API, API Яндекс Карт, MapBox, OpenStreetMap и др.

- https://www.mapbox.com
  - регистрируемся на сайте  
    `https://account.mapbox.com/auth/signup/`
  - подтверждаем email (переходим по ссылке, которая пришла на почту)
  - получаем Access token  
    `https://account.mapbox.com/`
  - выбираем понравившийся дизайн  
    `https://docs.mapbox.com/mapbox-gl-js/examples/`
  - [API Docs](https://docs.mapbox.com/api/maps/)

**6. Геокодирование**  
Google Geocoding, Яндекс.Карты Геокодирование, Nominatim OpenStreetMap, Data Science Toolkit, Gisgraphy, OpenCage Geocoder и др.

- https://opencagedata.com/
  - регистрируемся на сайте
  - получаем API key
  - получаем координаты по названию населённого пункта  
    `https://api.opencagedata.com/geocode/v1/json?q=Minsk&key=c6b6da0f80f24b299e08ee1075f81aa5&pretty=1&no_annotations=1`
  - [API Docs](https://opencagedata.com/api)
    </details>
