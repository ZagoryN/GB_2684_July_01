## Работа с ветками, создание

Чтобы вывести список всех веток на экран, мы используем команду:
+ **git branch**

Чтобы изменить название ветки, нужно _находиться в ней_ и прописать 
- **git branch** -m "new_name"

Чтобы создать новую ветку, мы используем:
+ **git branch branch_name** - создается ветка с именем branch_name

## Работа с ветками, продолжение

Чтобы переходить между ветками необходимо использовать команду 
+ **git checkout Branch_Name**

Есть также сокращенная команда, позволяющая одновременно создать и перейти на новую ветку (актуальная ветка отмечается знаком * )
- **git checkout -b New_branch_name**

Чтобы просмотреть историю изиенений, с учетом изменений и слияний веток, необходимо использовать команду:
+ **git log --graph**

## Работа с ветками, конец работы с веткой

Когда работа над веткой частично закончена или полностью готова, необходимо перенести выполненную работу в ветке в текущую, основную версию с помощью команды:
+ **git merge branch_name**

***Важное примечание***: слияния веток необхоимо прозводить из родительской ветки, т.е. если веток другого уровня нет, то из ветки <ins>master</ins>. 

Когда работа с веткой завершена, и ветка более не понадобится, можно удалить ветку с помощью следующих команд:

+ **git branch -d branch_name**
+ **git branch -D branch_name**

отличие этих команд в флаге: 
1. <ins>-d</ins> перед удалением проверяет наличие слияния, объединена ли она? Аналог корзины на рабочем столе.
2. <ins>-D</ins> удаляет ветку без проверок.

## Работа с удаленными репозиториями
Начать работу необходимо с копирования/клонирования репозитория с сервиса GitHub, делается с помощью команд:

* **git remote add origin** <https://..........>
* **git clone** <https://..........>

Получить ссылку на свой репозиторий можно, нажав кнопку "Code", ссылка на чужой репозиторий получается по кнопке "Fork".

Если работа изменена с другого устройства или через GitHub, необходимо применить команду :
* **git pull**

**git pull** является составной командой и одновременно скачивает актуальное состояние репозитория (git fetch) и производит слияние (git merge).

> Например, строки 47-50 (информация о git pull) были изменены на GitHub и скачаны на локальный репозиторий.

А чтобы с локального репозитория выполненные изменения или работа целиком отобразились на сервисе, необходимо использовать команду для выгрузки содержимого локального репозитория в удаленный:
- **git push**









 
