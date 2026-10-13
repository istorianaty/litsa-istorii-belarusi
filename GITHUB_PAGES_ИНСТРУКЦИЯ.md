# Как разместить игру на GitHub Pages через GitHub Desktop (Windows)

## Вариант А. Если репозитория еще нет

1. Распакуйте ZIP-файл в удобное место, например `Документы\GitHub\litsa-istorii-belarusi`.
2. Запустите **GitHub Desktop** и войдите в свою учетную запись GitHub.
3. Выберите **File → Add local repository → Choose…** и укажите распакованную папку `litsa-istorii-belarusi`.
4. Поскольку эта папка пока не содержит Git-репозитория, GitHub Desktop может предложить **Create a repository here** — нажмите эту ссылку. Если такого предложения нет: выберите **File → New repository**, задайте имя `litsa-istorii-belarusi`, создайте репозиторий, а затем скопируйте файлы из распакованной папки внутрь созданного репозитория.
5. В поле **Summary** напишите, например, `Первая версия игры`, нажмите **Commit to main** (если файлы еще не закоммичены).
6. Нажмите **Publish repository**. Для открытого сайта отключите **Keep this code private**; затем подтвердите **Publish Repository**.
7. В GitHub Desktop выберите **Repository → View on GitHub**, чтобы открыть репозиторий на сайте.
8. На сайте GitHub откройте **Settings → Pages**.
9. В блоке **Build and deployment → Source** выберите **Deploy from a branch**.
10. В поле **Branch** выберите `main`, рядом — `/(root)`, нажмите **Save**.
11. Дождитесь публикации. Когда GitHub Pages покажет ссылку **Visit site**, откройте ее и проверьте игру.

Адрес обычно выглядит так: `https://ВАШ-ЛОГИН.github.io/litsa-istorii-belarusi/`.

## Вариант Б. Если репозиторий уже создан

1. Откройте репозиторий в **GitHub Desktop** и выберите **Repository → Show in Explorer**.
2. В проводнике Windows откройте папку этого репозитория. Скопируйте в нее **содержимое** архива: `index.html`, `README.md`, `.nojekyll`, `.gitignore`, `images` и обе инструкции. `index.html` должен находиться прямо в корне, а не внутри второй вложенной папки.
3. Вернитесь в GitHub Desktop: слева появятся измененные файлы.
4. Введите Summary `Обновление игры` и нажмите **Commit to main**.
5. Нажмите **Push origin**. Если репозиторий еще не опубликован — **Publish repository**.
6. Проверьте публикацию через **Settings → Pages** на сайте GitHub.

## Как обновлять игру в дальнейшем

Замените `index.html` новой версией, затем **Commit to main → Push origin**. Ссылка на игру при этом останется прежней.

## Важные нюансы

- ZIP-файл **не нужно загружать как единственный файл репозитория**: сначала распакуйте его. GitHub Pages ищет `index.html` в выбранной папке публикации.
- Сайт на GitHub Pages требует интернет-соединения для первоначального открытия. Для офлайн-работы используйте сохраненный `index.html`.
- Игра сохраняет достижения и результаты **локально в браузере**; при переходе с локального файла на адрес GitHub Pages прежние результаты не переносятся автоматически.
- Если «Visit site» не появляется сразу, проверьте в разделе **Actions**, завершилось ли развертывание, и подождите несколько минут.
- Для публичной публикации заранее проверьте условия использования исторических иллюстраций. См. `ИСТОЧНИКИ_И_ПРАВА.md`.

Официальная документация:
- https://docs.github.com/en/desktop/overview/creating-your-first-repository-using-github-desktop
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
