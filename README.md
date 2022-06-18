# Git_Merg_Branch

GitHub. HW_2

0. Создать репозиторий на GitHub и выгрузить на локальный GitHub
Git_Merg_Branch

Git clone https://github.com/svetylka/Git_Merg_Branch.git
1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

Git branch

Git branch Postman

Git branch Jmeter

Git branch CheckLists

Git branch BagReports

Git branch SQL

Git branch Charles

Git branch Mobile_testing

2. Запушить все ветки на внешний репозиторий

git push origin Postman Jmeter CheckLists BagReports SQL Charles Mobile_testing

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта

git checkout BagReports

cat >> BugReports.txt

ID: VKs-1111
Author: Aleksa
Assignment: Aleksa
Priority: Very High
Title: [Ошибка] Preprod. Кнопка регистрации не октивна на странице регистрации 
Environment: Preprod. Google Chrome version 110
Preconditions: Открыть страницу https://xyz.com , перейти в раздел регистрации
STR: Заполнить Иванов Иван Иванович, дата рождения 10.02.1990г. и нажать кнопку зарегистрироваться
ER: Регистрация успешно выполнена и на почту пришло письмо об успешной регистрации 
AR: Кнопка регистрации не активна после заполнения всех необходимых полей регистрации 
Attachments: Screenshot-001.png , Skreencast-001.mp4
git add . && git commit -m "add BagReports"

4. Запушить структуру багрепорта на внешний репозиторий

git push --set-upstream origin BagReports

5. Вмержить ветку Bag Reports в Main

git checkout main

git marge BagReports -m "merge BugReports"
6. Запушить main на внешний репозиторий.
git push

7. В ветке CheckLists набросать структуру чек листа.
git checkout checklists

cat >> checklist.txt

1. Проверить запуск приложения на Preprod
2. Установить приложения из тестового репозитория 
3. Удалить приложение
4. Удалить приложение из внутреннего тестового маркет плейса
5. Удалить приложение из маркет плейса

git add . && git commit -m "add checklist"

8. Запушить структуру на внешний репозиторий
git push --set-upstream origin checklist
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

Нажать на Pull Request в GitHub и выбрать ветки CheckLists в main
10. Синхронизировать Внешнюю и Локальную ветки Main
git fetch
git pull
