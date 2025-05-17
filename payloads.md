# Payloads для gruyere

_Пример оформления работы_

## Payload 1

При переходе по ссылке `https://example.com/example`. Параметр `example` можно заменить на пейлоад `<script>alert(document.cookies)</script>` для выполнения Reflected XSS инъекции в элементе `<div id="search-query-param">...</div>`, который покажет куки файлы пользователя

## Payload 2

При создании New Snippet в поле вставить `<img src=1 onerror=alert(Hi)>`, алерт будет выполняться каждый раз, когда пользователь, будет заходить на главную страницу или страницу "Snippets".

## Payload 3

При вставке `<script>alert(1)</script>` на главной станице после url, выводится алерт.

## Payload 4

При наведении курсор выводится алерт, если в поле Profile Color встатвить `blue'onmouseover='alert(blue)`.

## Payload 5

После авторизации в url можно вставить `<script>alert('Hi')</script>`, выводится алерт.

## Payload 6
После создания New Snippet в url можно вставить `deletesnippet?index=0` для удаления сниппетов.
