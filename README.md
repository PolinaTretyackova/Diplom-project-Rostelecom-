# Итоговая работа на форме авторизации Ростелеком 

Объект тестирования: https://b2c.passport.rt.ru


1. Ссылка на текст-кейсы: https://docs.google.com/spreadsheets/d/16bYzlLgvtQyHUqaK9uLR6btpp1-hNe3M57F26IdqE2g/edit?usp=sharing
2. Автоматизированные тесты вложены на GitHub.
3. Баг:

- Во время тестирования странцы сайта зависали. Особенно во время запуска всех тестов и на середине запущенного теста страница регистрации сайта выходила ошибка и тем самым тест проваливался. Но если запускать тест отдельно, тест проходил успешно.
- При тестировании "Проверка названия кнопки "Продолжить" в форме "Регистрация"" тест не прошел, выходит ошибка.
- Баги описаны: https://docs.google.com/spreadsheets/d/1JlklezBfrZ7u4vlb4XK83NZdLzflwspZc8A2gn7l36g/edit?usp=sharing

Тестирование приходило на основе pytest-selenium. Данным инструментом проверялась авторизация и регистрация на сайте. Выбран этот иснтрумент из-за простоты использования и получения точных результатов.

- Тест запущен с помощью pytest -v --driver Chrome --driver-path /mvideo-/Desktop/chrome/chromedriver.exe tests_rost.py
- Использован webdriver для Chrome версия 110.0.5481.77

test_rost - описаны тесты settings - необходимые данные для теста
