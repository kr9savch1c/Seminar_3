# Справка (туториал) по основам системы контроля версий GIT

## Что такое GIT?
**GIT** - это одна из реализаций распределённых систем
контроля версий, имеющая как и локальные, так и
Удалённые репозитории. Является самой популярной
реализацией систем контроля версий в мире.

## Как инициализировать GIT
**Чтобы инициализировать репозиторий, необходимо прописать в терминале следующую команду:**

```
git init
```

## Создание коммитов в GIT

### git add
Команда **git add** добавляет файл в репозиторий GIT'a, с указанием имени файла. Полная команда выглядит так:
```
**git add <имя_файла>**
```

### Проверка статуса репозитория
Команда **git status** проверяет статус репозитория. С помощью этой команды можно проверить были ли изменения в файлах.

### Создание комментариев
Команда **git commit -m "комментарий"** добавляет комментарий к последней фиксации файла. Есть универсальная команда с фиксацией файла и комментарием к нему:
```
**git commit** -am "комментарий" - a - add, m - комментарий.
```

# Туториал(справка) для работы с языком разметки Markdown








## Заголовки
Заголовки отмечаются диезом `#` в начале строки, от одного до шести. Например:

# Заголовок первого уровня #
## Заголовок h2
### Заголовок h3
#### Заголовок h4
##### Заголовок h5
###### Заголовок h6

В декоративных целях заголовки можно «закрывать» с обратной стороны.

## Цитаты
Цитаты оформляются как в емейлах, с помощью символа `>`.

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

Или более ленивым способом, когда знак `>` ставится перед каждым элементом цитаты, будь то абзац, заголовок или пустая строка:

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

В цитаты можно помещать всё что угодно, в том числе вложенные цитаты:

> ## This is a header.
>
> 1.   This is the first list item.
> 2.   This is the second list item.
>
> > Вложенная цитата.
>
> Here's some example code:
>
>     return shell_exec("echo $input | $markdown_script");


## Исходный код
В чистом Маркдауне блоки кода отбиваются 4 пробелами в начале каждой строки.

Но в GitHub-Flavored Markdown (сокращенно GFM) есть более удобный способ: ставим по три апострофа (на букве Ё) до и после кода. Также можно указать язык исходного кода.

```python
async def chiter(ctx):
    await ctx.send("Привет, земляне, я бот Толика Царапкина") 
```

## Таблицы
В чистом Маркдауне нет синтаксиса для таблиц, а в GFM есть.

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

Для красоты можно и по бокам линии нарисовать:

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

Можно управлять выравниванием столбцов при помощи двоеточия.

| Left-Aligned  | Center Aligned  | Right Aligned |
|:------------- |:---------------:| -------------:|
| col 3 is      | some wordy text |     **$1600** |
| col 2 is      | centered        |         $12   |
| zebra stripes | are neat        |        ~~$1~~ |

Внутри таблиц можно использовать ссылки, наклонный, жирный или зачеркнутый текст.

Для всего остального есть обычный HTML.