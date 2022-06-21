## Переменные с префиксами
При подключении модуля Kalium19 через директиву `@use` можно указать дополнительные ~~параметры~~ переменные, как например:

```scss
@use 'path/to/kalium19` as k19 with (
  $prefixes_border-radius: webkit
)
```

А т.к. при использовании некоторых миксинов нам не нужны дополнительные префиксы, допустим для Firefox, то было бы хорошо, если Kalium19 не генерировал префиксы к определенным миксинам или генерировал только те, что ныжны именно вам.

Ниже расположен весь список переменных со списком префиксов для миксинов:
- `$prefixes_border-radius: webkit moz`
- `$prefixes_animation: o ms moz webkit`
- `$prefixes_background-size: o moz webkit`
- `$prefixes_box-shadow: webkit moz`
- `$prefixes_box-sizing: webkit moz o`
- `$prefixes_column-count: moz webkit`
- `$prefixes_column-gap: moz webkit`
- `$prefixes_box-align: webkit moz`
- `$prefixes_align-items: webkit`
- `$prefixes_flex-basis: webkit`
- `$prefixes_flex-direction: webkit ms`
- `$prefixes_box-direction: webkit moz`
- `$prefixes_flex-flow: webkit ms`
- `$prefixes_box-flex : webkit moz`
- `$prefixes_flex-grow: webkit`
- `$prefixes_box-pack: webkit moz`
- `$prefixes_justify-content: webkit`
- `$prefixes_box-ordinal-group: webkit moz`
- `$prefixes_order: webkit`
- `$prefixes_flex-shrink: webkit moz`
- `$prefixes_opacity: moz khtml`
- `$prefixes_tab-size: o moz`
- `$prefixes_transform: o ms moz webkit`
- `$prefixes_transform-origin: o ms moz webkit`
- `$prefixes_transform-style: moz webkit`
- `$prefixes_transition: o moz webkit`

Получается, что если нам нужно оставить только поддержку Firefox для свойств `border-radius`, `box-shadow` и `opacity`, то наш код будет выгляеть так:

```scss
@use 'path/to/kalium19` as k19 with (
  $prefixes_border-radius: moz,
  $prefixes_box-shadow: moz,
  $prefixes_opacity: moz
)
```
