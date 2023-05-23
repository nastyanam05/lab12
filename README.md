# lab12
Устанавливаю Vim: `brew install vim`
Перехожу в тутор: `vimtutor ru`
* Перемещение на `hjkl` ;
* Для выхода без сохранения Esc(Normal mod) `:q!` ;
* Удаляет символ — `x` ;
* Вставка — `i` ;
* Добавление — `A` ;
* Для выхода с сохранением — `:wq` ;
* Для запуска файла `Vim <имя файла>` ;
* Удалить слово `dw` ;
* Удалить строку `d$` ;

Список объектов:
```
    w - от курсора до конца слова, включая последующий пробел.

    e - от курсора до конца слова, НЕ включая последующий пробел.

    $ - от курсора до конца строки.

    ^ - от курсора до начала строки.
```
* Перемещение на n слов `nw` вперёд и `0` для перемещения в начало строки ;
* Удаление n слов `dnw` ;
* Удаление строки `dd` ;
* Отмена `u`, `U` ;
* Откат отмены `CTRL-R` ;
* Вставка текста, который был только что удален `p` ;
* Замена символа `r` ;
* `Ctrl-g`  показывает ваше положение в файле и информацию о нем ;
* `Shift-G`  перемещает вас в конец файла ;
* Поиск слова `/<слово>` , листать вперёд `n`, листать назад `N`, поиск слова назад `?<слово>` ;
* Нажатие  `%` , когда курсор находится на (,),[,],{, или } позволяет найти парную скобку ;
* Для подстановки стало вместо всех было в строке, наберите `:s/было/стало/g` ;

 Поиск и замена слова `:s<слово_для_замены>/<заменяемое_слово>`
 ```
:#,#s/было/стало/g  где #,# -- номера этих строк.

:%s/было/стало/g    для замены всех вхождений во всем файле.

:%s/было/стало/gc   для поиска всех вхождений во всем файле и запроса подтверждения замены.
```
* `:!` команда  исполняет внешнюю команду ;
* `:!ls` выводит файлы в текущем каталоге ;
* `:w <имя_файла>` сохраняет файл ;
* `:!rm <имя_файла>` удаляет файл ;
* Нажмите  `o`  для создания строки НИЖЕ курсора и перехода в режим вставки ;
  Нажмите  `O`  для создания строки ВЫШЕ курсора ;
* Нажмите  `a`  для вставки текста ПОСЛЕ курсора ;
  Нажмите  `A`  для вставки текста в конец строки ;
* Команда  `e`  подводит курсор к концу слова ;
* Команда  `y`  копирует текст,  `p`  -- вставляет скопированный текст ;
* Нажатие заглавной  `R`  переводит в режим замены до нажатия клавиши  <ESC> ;
* Наберите `:set xxx` для включения параметра `xxx`, некоторые параметры:
	
```
ic	ignorecase	игнорирование регистра при поиске
is	incsearch	отображение частичных совпадений при поиске
hls	hlsearch	подсветка всех совпадений при поиске
```
	
* Добавьте no перед параметром для его отключения:  `:set noic` ;
* `:help` для справки.
