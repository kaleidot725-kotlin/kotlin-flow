# Exeption Transparency

- Catch オペレータで例外をキャッチできる。
- catch した場合にエラー値を emit しなければならない

## Transparent catch

- Catch オペレータは上位の Flow の例外のみをキャッチする

## Catching declaratively

- onEach にて check し、 catch で例外をキャッチすることもできる。
