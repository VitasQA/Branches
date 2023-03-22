🗲**Branches🗲**

*Задание 1. На локальном репозитории сделать ветки для:*
+ *Postman*
+ *Jmeter* 
+ *CheckLists* 
+ *Bug Reports*
+ *SQL* 
+ *Charles* 
+ *Mobile testing* 

`Решение`⮯

1. Посмотреть на какой ветке в данный момент:
   
```bash
git branch
```

2. Создать ветки:

```bash
git branch Postman
git branch Jmeter
git branch CheckLists
git branch Bug_Reports
git branch SQL
git branch Charles
git branch Mobile_testing
```

ИЛИ

```bash
git branch Postman && git branch Jmeter && git branch CheckLists && git branch Bug_Reports && git branch SQL && git branch Charles && git branch Mobile_testing
```
---

*Задание 2. Запушить все ветки на внешний репозиторий.*

`Решение`⮯

```bash
git push -u origin --all
```
---

*Задание 3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта.*

`Решение`⮯

1. Перейти в ветку:

```bash
git checkout Bug_Reports 
```

2. Создать текстовый документ:

```bash
cat > bug_report.txt
```

ИЛИ

```bash
vim bug_report.txt
```

Используем cat:

3. Ввести:

```txt
1. ID
2. Summary 
3. Priority
4. Severity
5. Environment
6. Precondition
7. Steps to Reproduce
8. Postcondition
9. Expected result
10. Actual result
11. Attachments
12. Status
```

4. Нажать "Enter"
5. Нажать "CTRL + D"

Кроме того, можно использовать в одну строку:

```bash
git checkout Bug_Reports && cat > bug_report.txt
```
---

*Задание 4. Запушить структуру багрепорта на внешний репозиторий.*

`Решение`⮯

```bash
git add .
git commit -m "add bug_report.txt"
git push
```
---

*Задание 5. Вмержить ветку Bug Reports в Main.*

`Решение`⮯

1. Перейти в ветку main:

```bash
git checkout main
```

2. Выполнить слияние веток:

```bash
git merge Bug_Reports
```
---

*Задание 6. Запушить main на внешний репозиторий.*

`Решение`⮯

```bash
git add .
git commit -m "add Bug_Report.txt"
git push
```
---

*Задание 7. В ветке CheckLists набросать структуру чек листа.*

`Решение`⮯

1. Ввести:
   
```bash
git checkout CheckLists && cat > checklist.txt
```

2. Ввести информацию:

```txt
1. Task ID
2. Task Title
3. Task Status
```

3. Нажать "Enter"
4. Нажать "CTRL + D"
---

*Задание 8. Запушить структуру на внешний репозиторий.*

`Решение`⮯

```bash
git add .
git commit -m "add checklist.txt"
gut push
```
---

*Задание 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main:*

`Решение`⮯

1. Зайти в ветку CheckLists
2. Нажать "Compare && Pull requests" -> Pull request successfully merged and closed
---

*Задание 10. Синхронизировать Внешнюю и Локальную ветки Main.*

`Решение`⮯

```bash
git checkout main
git pull
```
