# __Действия с файлами репозитория__

## __Создание и добавление файла в репозиторий__
Чтобы создать и добавить файл в репозиторий:
1. Создайте markdown-файл в каталоге проекта.
1. Внесите необходимые изменения и сохраните файл.
1. Можно проверить  текущее состояние репозитория с помощью команды `git status`. Выводится состояние «Untracked files» — в проекте появились неотслеживаемые файлы.
1. Добавьте изменения в индекс (проиндексируйте):
    * в командной строке выполните команду `git add <путь_до_файла>`;
    * в VS Code в левой панели перейдите на вкладку __Source Control__ и нажмите __+__ у имени файла.
1. Можно проверить текущее состояние репозитория с помощью команды `git status`. Выводится состояние «Changes to be committed» — изменения файла попали в индекс.
1. Зафиксируйте изменения с помощью коммита (закоммитьте):
    * в командной строке выполните команду `git commit -m «описание_изменений»`;
    * в VS Code в левой панели перейдите на вкладку __Source Control__, затем введите описание изменений в поле и нажмите кнопку __Commit__.
1. Можно проверить текущее состояние репозитория с помощью команды `git status`. Выводится состояние «nothing to commit, working tree clean» — репозиторий не содержит измененных файлов после последнего коммита.
1. Перенесите изменения из локального репозитория в удаленный. По умолчанию данные будут передаваться из текущей ветки в ту же ветку удаленного репозитория:
    * в командной строке выполните команду `git push -u origin <название_ветки>`;
    * в VS Code в левой панели перейдите на вкладку __Source Control__ и нажмите кнопку __Sync Changes__.
<br>

# __Внесение изменений в файлы репозитория__

## __Изменение файла проекта__
Чтобы изменить файл проекта:
1. Добавьте изменения и сохраните markdown-файл.
1. Можно проверить текущее состояние репозитория с помощью команды `git status`. Выводится состояние «Changes not staged for commit» — отслеживаемый файл изменен, но не проиндексирован.
1. Добавьте изменения в индекс (проиндексируйте):
    * в командной строке выполните команду `git add <путь_до_файла>`;
    * в VS Code в левой панели перейдите на вкладку __Source Control__ и нажмите кнопку __+__ у имени файла.
1. Можно проверить текущее состояние репозитория с помощью команды `git status`. Выводится состояние «Changes to be committed» — изменения файла попали в индекс.
1. Добавьте изменения из индекса в репозиторий (закоммитьте):
    * в командной строке выполните команду `git commit -m «описание_изменений»`;
    * в VS Code в левой панели перейдите на вкладку __Source Control__, затем введите описание изменений в поле и нажмите кнопку __Commit__.
1. Можно проверить текущее состояние репозитория с помощью команды `git status`. Выводится состояние «nothing to commit, working tree clean» — репозиторий не содержит измененных файлов после последнего коммита.
1. Перенесите изменения из локального в удаленный репозиторий. По умолчанию данные будут передаваться из текущей ветки в ту же ветку удаленного репозитория: 
    * в командной строке выполните команду `git push origin <название_ветки>`;
    * в VS Code в левой панели перейдите на кладку __Source Control__ и нажмите кнопку __Sync Changes__.
<br>

## __Внесение изменений в чужой репозиторий__
Если изменения были отправлены в чужой репозиторий, то дополнительно необходимо создать пулреквест:
1. Войдите в аккаунт на GitHub и откройте репозиторий.
1. Создайте пулреквест: нажмите __Compare&pull request__.
1. Добавьте описание изменений и нажмите __Create pull request__.
<br>