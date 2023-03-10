[<- к содержанию](readme.md)

## Просмотр изменений

Если результат работы команды `git status` недостаточно информативен для вас — вам хочется знать, что конкретно поменялось, а не только какие файлы были изменены — вы можете использовать команду `git diff`. Если `git status` отвечает на эти вопросы в самом общем виде, перечисляя имена файлов, `git diff` показывает вам непосредственно добавленные и удалённые строки — патч как он есть.

Команда `git diff` сравнивает содержимое вашего рабочего каталога с содержимым индекса. Результат показывает ещё не проиндексированные изменения.

Если вы хотите посмотреть, что вы проиндексировали и что войдёт в следующий коммит, вы можете выполнить `git diff --staged`. Эта команда сравнивает ваши проиндексированные изменения с последним коммитом.

Важно отметить, что `git diff` сама по себе не показывает все изменения сделанные с последнего коммита — только те, что ещё не проиндексированы. Такое поведение может сбивать с толку, так как если вы проиндексируете все свои изменения, то `git diff` ничего не вернёт.