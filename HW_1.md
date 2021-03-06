## git_branches

- [X] **GitHub. HW_1**

1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

```
git branch Postman
git branch Jmeter
git branch CheckLists
git branch BugReports
git branch SQL
git branch Charles
git branch Mobile_testing
```
2. Запушить все ветки на внешний репозиторий

```
git push origin --all
```
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта

```
git checkout BugReports
touch BugReport_structure.txt
```

```
vim BugReport_structure.txt
i
```

|№|Summary|Description|Steps to reproduce|Environment|Reproducibility|Severity|Priority|
|-------------|:------:|-----|----|---|--|--|--|
| | | | | | | | | |

```
Esc
:wq
```
4. Запушить структуру багрепорта на внешний репозиторий

```
git add BugReport_structure.txt
git commit -m "add file BugReport_structure.txt"
git push --set-upstream origin BugReports
```
5. Вмержить ветку Bug Reports в Main

```
git checkout main
git merge BugReports
```
6. Запушить main на внешний репозиторий.

```
git push origin main
```

7. 7. В ветке CheckLists набросать структуру чек листа.

```
git checkout CheckLists
touch CheckList.txt
```

```
vim CheckList.txt
i
```
|Test Readiness Review|Status|
|-------------|:------:|
| All the Requirements finalized| Done |
|Test Plan created and reviewed|Done|
|Test Cases preparation done|Done|
|Test Case review and sign off|Done|
|Test Data availability|Done|
|Smoke Testing	|Done|

```
Esc
:wq
```

8. Запушить структуру на внешний репозиторий

```
git add CheckList.txt
git commit -m "add file CheckList.txt"
git push --set-upstream origin CheckLists
```
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

```
На интерфейсе гитхаба:
	Compare & Pull request -> Create pull request
	->Merge pull request -> Congfirm Merge
```

10. Синхронизировать Внешнюю и Локальную ветки Main

```
git pull
```


-------
Ссылка на задание 2: https://github.com/ping335/git_2
