# lang-uk_UA

### ПРОЧИТАЙТЕ ЦЕ, КОЛИ ВИ ХОЧЕТЕ ЗРОБИТИ ПЕРЕКЛАДИ ІНШОЮ МОВОЮ

У цьому сховищі міститься шістнадцять основних текстових файлів, кожен із власним розділом перекладів:

- translations.txt -- це загальні переклади, які завантажуються щоразу
- helptext.txt -- це всі розділи довідкового тексту, які завантажуються щоразу
- dashboard.txt -- це переклади для розділу інформаційної панелі
- main.txt -- це переклади основного розділу
- shares.txt -- це переклади розділу shares
- users.txt -- це переклади для розділу користувачів
- settings.txt -- це переклади розділу налаштувань
- plugins.txt -- це переклади розділу плагінів
- docker.txt -- це переклади розділу docker
- vms.txt -- це переклади розділу vms
- tools.txt -- це переклади розділу інструментів
- javascript.txt -- це переклади для сценаріїв javascript
- scripts.txt -- це переклади для локальних скриптів
- apps.txt -- це переклади для розділу CA (у папці Community Apps)
- ca_settings - це переклади налаштувань ЦС (у папці Community Apps)
- javascript.ca.txt-- це переклади для CA javascript (у папці Community Apps)

Усі назви файлів пишуться у нижньому регістрі та повинні бути включені в репозиторій, щоб переклади були повними.

Видалення певного файлу означає, що переклади для цього розділу не будуть доступні, а графічний інтерфейс відображатиме текст оригінальною англійською мовою.

### ПЕРЕКЛАДИ

Кожен текстовий файл містить звичайні текстові рядки, що зберігаються у форматі UTF-8 із закінченнями рядків Linux.
Використовуйте текстовий редактор, який підтримує формат UTF-8 і linux, наприклад [notepad++](https://notepad-plus-plus.org/downloads)

Вміст кожного текстового файлу розділений на дві частини

### ЧАСТИНА 1

Це однорядкові записи у форматі:

`оригінал англійського тексту = перекладений іноземний текст`

Змініть текст лише після знака рівності (=) і залиште оригінальний англійський текст ліворуч.
Видалення рядка або пропуск перекладу після знака рівності призводить до того, що графічний інтерфейс відображає цей рядок з оригінальним англійським текстом.

Перекладений текст може містити «спеціальні символи», такі як косі риски, дужки або дужки, які не входять до основного тексту,
але які використовуються для відображення тексту відповідно. напр.

`Параметри див. Help=Options (див. Довідку)`

Символи \* і \*\* використовуються для відображення тексту курсивом і жирним шрифтом відповідно. напр.

`Масив має бути зупинений для зміни=Масив має бути **зупинений** для зміни`

Рекомендується робити переклади на розділ, тобто по одному файлу за раз, і перевіряти правильність перекладів у графічному інтерфейсі.
перш ніж перейти до наступного розділу.

Пам’ятайте про довжину перекладів і намагайтеся зробити їх такою ж довжиною, як і оригінальний текст, і уникайте проблем з простором у графічному інтерфейсі.

### ЧАСТИНА 2

Це багаторядкові записи, які використовуються для одночасного перекладу кількох рядків.
Багаторядковий переклад має унікальний відкриваючий і закриваючий тег:

**:unique_tag_name_plug:** - унікальний початковий тег, який використовується для будь-якого багаторядкового текстового розділу

**:end** - закриваючий тег

Не видаляйте і не змінюйте ці теги, а перекладайте лише текст між початковим і закриваючим тегами!

### ТЕКСТ ДОПОМОГИ

Весь текст довідки GUI зберігається в одному файлі *helptext.txt*.

Цей файл має кілька розділів довідкового тексту. Кожен розділ укладено унікальним відкриваючим тегом і відповідним закриваючим тегом.

**:unique_tag_name_help:** - унікальний початковий тег, який використовується для текстового розділу довідки

**:end** - відповідний закриваючий тег

Не видаляйте і не змінюйте ці теги, а перекладайте лише текст між початковим і закриваючим тегами!

Майте на увазі, що використовується синтаксис стилю Markdown, його потрібно зберегти.

### ЛОКАЛЬНЕ ТЕСТУВАННЯ

Коли переклади завершені, і ви хочете локально перевірити (проміжні) результати, текстові файли потрібно заархівувати в один ZIP-файл.
Дайте файлу ZIP назву вашої мови, напр. French.zip.

У графічному інтерфейсі перейдіть до: Інструменти -> webGUI -> Мова (перейдіть до перегляду розробника)

- За замовчуванням встановлюється лише англійська мова (вбудована)
- Виберіть файл ZIP, який ви створили раніше, як вихідний файл
- Якщо назва мови розпізнається, вона буде вибрана автоматично, в іншому випадку виберіть назву мови зі спадного меню для встановлення.
- Натисніть «Завантажити», щоб додати ваші переклади до графічного інтерфейсу під назвою вибраної мови

ПРИМІТКА. Якщо ваша мова недоступна у спадному меню, надішліть запит на [форумі Unraid](https://forums.unraid.net/forum/75-multi-language-section/)

Тепер ваша мова доступна для локального тестування!

У графічному інтерфейсі перейдіть до: Налаштування -> Налаштування дисплея -> Мова

- Виберіть бажану мову зі спадного меню. Зауважте, що тут відображаються лише доступні варіанти мов.

### GITHUB

Репозиторій мов буде доступний на [Github](https://github.com/unraid), де перекладачі можуть створювати Pull Requests (PR) і надсилати свою роботу.

Як тільки ви будете задоволені своїми результатами, використовуйте Github (потрібен обліковий запис), щоб розділити відповідний репозиторій мов і створити PR зі своїми змінами.

Limetech розгляне це та об’єднає вашу роботу після схвалення.

### ОНОВЛЕННЯ

Коли оновлені вихідні текстові файли англійською мовою стануть доступними в майбутньому, ці оновлення стануть доступними через Github.

Перекладачі можуть використовувати систему Github, щоб побачити, які зміни внесені, і відповідно оновити свої переклади.

### КРЕДИТИ

Ми вітаємо ваші зусилля, і щоб показати нашу вдячність, ваше ім’я та мова вказано на сторінці «Кредити» в розділі «Інструменти» в графічному інтерфейсі.
Будь ласка, повідомте нам, які облікові дані використовувати.

Дуже дякую!
