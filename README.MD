# План тестирования записи на обучение профессии "Тестировщик ПО"
## 1. Перечень автоматизируемых сценариев:
### *1.1 Переход к форме записи на курс*
> **а. Переход к форме записи на курс с главной страницы через «Каталог курсов» с помощью вкладки «Программирование»**

- На главной странице нажать «Каталог курсов»
- В выпадающем списке навести курсор на раздел «Программирование»
- В выпадающем списке нажать на «Тестировщик ПО»
- В открывшейся странице нажать кнопку «Записаться»
- Заполнить открывшуюся форму валидными данным
- Нажать на кнопку Записаться

> **б. Переход к форме записи на курс с главной страницы через «Каталог курсов» с помощью вкладки «Полный каталог»**

- На главной странице нажать «Каталог курсов»
- В выпадающем списке навести курсор на раздел «Программирование»
- В выпадающем списке нажать на «Тестировщик ПО»
- В открывшейся странице нажать кнопку «Записаться»
- Заполнить открывшуюся форму валидными данным
- Нажать на кнопку Записаться

> **в. Переход к форме записи на курс с главной страницы в разделе «Направления обучения»**

- На главной странице нажать на раздел «Программирование»
- В списке нажать на «Тестировщик ПО»
- В открывшейся странице нажать кнопку «Записаться»
- Заполнить открывшуюся форму валидными данным
- Нажать на кнопку Записаться

### *1.2 Проверка отправки формы записи*
   
+ Успешная отправка: заполнение полей валидными данными
   + Ожидаемый результат: данные успешно отправлены. Появится всплывающее окно об успешном завершении записи


+ Отправка пустой формы
   + Ожидаемый результат: данные не отправляются. Под незаполненными полями появится сообщения "Поле обязательно для заполнения" 


+ Отправка формы с одним незаполненным полем
   + Ожидаемый результат: данные не отправляются. Под незаполненным полем появится сообщение "Поле обязательно для заполнения"


+ Валидация каждого из полей
   + Поле Имя должно состоять только из русских букв, дефисов и пробелов, минимум 2 символа
   + поле Телефон состоит только из 11 цифр, начинается с +7


## 2. Перечень используемых инструментов
   - Java - язык программирования
   - intellij idea - среда разработки для JAVA
   - Gradle - система автоматизации сборки
   - JUnit 5 - среда тестирования
   - Selenide - для тестирования WEB
   - Allure - для генерации отчета о тестировании
   - Docker - система контейнеризации


## 3. Перечень необходимых разрешений/данных/доступов
   - Разрешение от владльцев сайта на тестирование и автоматизацию
   - Разрешение на доступ к базе данных
## 4. Перечень и описание возможных рисков при автоматизации
   - При изменении верстки страницы сайта, потребуется корректировка всех автотестов, что займет много времени
## 5. Перечень необходимых специалистов для автоматизации
   - Один тестировщик
## 6. Интервальная оценка с учётом рисков (в часах)
   - Автоматизация проекта займёт примерно 24 рабочих часа