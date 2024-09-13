# Cypress-Autotests
<h2>Автотесты на UI с помощью JS + Cypress</h2>

> **Статус проекта:**
> Публичный проект: https://login.qa.studio/
> 
> 🟢 Поддерживается (активный) 

## Описание проекта и задачи
Автоматизировать часть проверок регресса с помощью Cypress

## Тест-кейсы, которые автоматизировали
* Авторизация с верным паролем и верным логином
* Авторизация c верным логином и неверным паролем
* Проверка работы валиадации на наличие @ в логине
* Проверка флоу восстановления пароля
* Проверка валидации
* Приведение к строчным буквам в логине (всегда проваливается)

## Детали реализации

1. baseUrl вынесен в переменные конфига
![image](https://raw.githubusercontent.com/QA-SirFourALot/Cypress-Autotests/main/BaseUrl.png)

2. Применение хуков beforeEach и afterEach
![image](https://raw.githubusercontent.com/QA-SirFourALot/Cypress-Autotests/main/Hooks.png)

3. Переменные данные для авторизации вынесены в отдельный файл
![image](https://raw.githubusercontent.com/QA-SirFourALot/Cypress-Autotests/main/Variables.png)

4. Каждая страница описана в формате объекта с локаторами
![image]()

## Локальный запуск тестов (из терминала)
1. Скачать проект
2. Перейти в терминале в директорию проекта
2. Выполнить команду:
```
npx cypress run --spec cypress/e2e/auth.cy.js --browser chrome
```
Ожидаемый результат: получим отчет о прохождении тестов.
![image](https://raw.githubusercontent.com/QA-SirFourALot/Cypress-Autotests/main/Terminal_launch.png)


## Локальный запуск через Cypress UI
1. Скачать проект и открыть в терминале.
2. Перейти в директорию проекта.
3. В терминале в папке с проектом запустить npm `install --save-dev cypress@12.7.0`
4. В терминале в папке с проектом запустить npm `npm i`
5. В терминале в папке с проектом запустить npm `npx cypress open`
6. Выбрать в Cypress UI E2E тестирование и браузер Google Chrome
7. Выбрать спеку auth

Ожидаемый результат: получим отчет о прохождении тестов.
![image](https://raw.githubusercontent.com/QA-SirFourALot/Cypress-Autotests/main/CypressUI_Laucnh.png)


## Автор

Клим Истомин ([@SirFouralot](https://t.me/SirFouralot))
