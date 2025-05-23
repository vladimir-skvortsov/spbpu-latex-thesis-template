# Шаблон LaTeX для выпускной квалификационной работы (ВКР) СПбПУ

Этот репозиторий содержит шаблон LaTeX, разработанный для соответствия требованиям к оформлению выпускных квалификационных работ (ВКР) в Санкт-Петербургском политехническом университете Петра Великого (СПбПУ).

Шаблон был успешно использован для подготовки [ВКР "Методология автоматизации проверок информационных моделей"](https://elib.spbstu.ru/dl/3/2023/vr/vr23-4010.pdf/info).

**Важно:** Хотя шаблон стремится соответствовать актуальным нормам контроля СПбПУ, рекомендуется сверяться с официальными требованиями вашего института/кафедры, так как они могут обновляться или иметь специфические дополнения. Вы можете адаптировать этот шаблон под конкретные нужды вашей работы.

Этот шаблон основан на [maks2199/DiplomaTeX](https://github.com/maks2199/DiplomaTeX).

**Ссылка на данный репозиторий:** [https://github.com/vladimir-skvortsov/spbpu-latex-thesis-template](https://github.com/vladimir-skvortsov/spbpu-latex-thesis-template)

## Ключевые особенности

* Структура, ориентированная на стандартные требования к ВКР СПбПУ.
* Разделение проекта на логические блоки: служебные файлы, ресурсы и контент.
* Предопределенные стили (`spbpu.sty`) для форматирования документа.
* Примеры пользовательских функций (`settings/myFunctions.tex`) для автоматизации некоторых аспектов верстки.
* Использование компилятора XeLaTeX для поддержки современных шрифтов и Unicode.

## Требования к системе

* **Компилятор:** XeLaTeX
* **Рекомендуемый редактор:** TeXstudio
* **Альтернативная среда:** Overleaf (необходимо выбрать компилятор XeLaTeX в настройках: Menu -> Compiler -> XeLaTeX).

## Структура проекта

Проект организован в три основные категории файлов:

1.  **Служебные файлы:** Отвечают за компиляцию документа, подключение настроек, стилей и пользовательских команд. Обычно не требуют модификации пользователем.
    * `main.tex`: Главный файл проекта, точка входа для компиляции. Объединяет все части документа.
    * `customFunctions.tex`: Содержит пользовательские LaTeX-функции для упрощения форматирования.
    * `spbpu.sty`: Файл стилей, определяющий внешний вид документа согласно требованиям СПбПУ.

2.  **Ресурсы:** Внешние файлы, используемые в документе.
    * `images/`: Директория для хранения изображений (рисунков, схем). Рекомендуется создавать подпапки для разных глав или типов изображений.
    * `pdfs/`: Директория для хранения PDF-файлов, которые необходимо включить в документ (например, приложения).
    * `bibliography.bib`: Файл библиографии в формате BibTeX. Содержит описания всех источников (книги, статьи, стандарты, веб-ресурсы), на которые есть ссылки в тексте.

3.  **Контент:** Файлы с непосредственным содержанием вашей работы (`.tex`). Структура контентных файлов в данном шаблоне соответствует общим рекомендациям для магистерских диссертаций СПбПУ, но может быть адаптирована.

## Использование шаблона

1.  **Клонируйте или скачайте** архив репозитория на ваш локальный компьютер.
2.  **Откройте проект** в вашем LaTeX-редакторе (рекомендуется TeXstudio) или загрузите файлы в Overleaf.
3.  **Убедитесь, что выбран компилятор XeLaTeX.** В TeXstudio это обычно настраивается в `Options -> Configure TeXstudio -> Build -> Default Compiler`. В Overleaf: `Menu -> Compiler -> XeLaTeX`.
4.  **Редактируйте файлы контента** (в основном, файлы `.tex` в корневой директории или поддиректориях, если вы их создадите). Наполняйте их текстом вашей ВКР, создавайте новые разделы и главы по мере необходимости.
5.  **Добавляйте изображения** в папку `images/` и ссылайтесь на них в тексте.
6.  **Добавляйте PDF-файлы** (если нужно) в папку `pdfs/`.
7.  **Заполняйте файл библиографии** `bibliography.bib` и используйте команды цитирования (`\cite`, `\citep`, и т.д.) в тексте.
8.  **Компилируйте проект**, запуская компиляцию файла `main.tex`. Обычно требуется несколько проходов компиляции для корректного отображения ссылок, библиографии и содержания.

## Вклад и предложения

Предложения по улучшению шаблона, исправления и сообщения об ошибках приветствуются.

* Пожалуйста, используйте раздел **Issues** в GitHub репозитории для сообщений об ошибках и запросов на новые функции.
* Для других вопросов или обсуждений можно связаться по электронной почте: `mail@vladimirskvortsov.com`.
