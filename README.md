# Todolist

Code-along: en todolista som sparas i webbläsaren. Den håller ihop allt från veckan: objekt i en array, DOM:en, händelser och event delegation.

## Kom igång

Öppna `index.html` med Live Server och öppna DevTools (F12). HTML:en och CSS:en är klara, och vi skriver JavaScripten i `js/main.js` steg för steg. Under **Application → Local Storage** ser du vad som sparas.

## Det här övar du på

- **Föränderlig data.** Arrayen `todos` ändras direkt med `push` och `splice`, och objekten i den ändras direkt.
- **Ett flöde efter varje ändring:** ändra datan, spara, rendera.
- **localStorage** med `JSON.stringify` och `JSON.parse`.
- **Rendera från data** med `createElement`, `textContent` och `replaceChildren`.
- **Event delegation:** en lyssnare på listan i stället för en per rad, med `closest` och `dataset`.
- Varför man tar bort baklänges i en loop.

## CSS:en

CSS:en följer ett system som är lätt att hitta i. Läs kommentaren överst i `css/index.css`.

| Lager | Exempel | Vad det styr |
| --- | --- | --- |
| Tokens | `--color-accent`, `--space-m` | Alla färger och avstånd, på ett ställe |
| Layout | `.container`, `.stack`, `.cluster` | Var saker ligger |
| Komponenter | `.button`, `.todo-item`, `.todo-item-text` | Hur saker ser ut |
| Varianter och lägen | `data-variant="ghost"`, `.is-done`, `:disabled` | Hur en komponent ser ut just nu |
| Utilities | `.visually-hidden`, `.gap-s` | En enda sak per klass |

Klasserna är på engelska och i kebab-case. Id:n är till för JavaScript och används aldrig i CSS:en.

## Bygg vidare

1. Dubbelklicka på en todo för att redigera texten.
2. Filtrera mellan Alla, Kvar och Klara. Filtret ska påverka renderingen, inte arrayen.
3. Mörkt läge: definiera om färgtokens i `@media (prefers-color-scheme: dark)`. Inget annat i CSS:en behöver ändras.
4. Vad händer om någon har skrivit skräp i localStorage? Gör `loadTodos` tålig med `try...catch`.

*// Sandra*
