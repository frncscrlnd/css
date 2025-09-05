# CSS?
Il CSS sta per Cascading Style Sheets, in italiano "Fogli di stile a cascata".
Il CSS è il linguaggio che serve per controllare l’aspetto di una pagina web.

Dice al browser come devono essere mostrati i contenuti HTML:

- Di che colore sono
- Che font hanno
- Quanto sono grandi
- Dove stanno nella pagina

Se hanno spazi, bordi, ombre, animazioni, ecc.
>[!IMPORTANT]
>🚫 Il CSS NON è un linguaggio di programmazione
>
>È un **linguaggio di stile (di formattazione)**.
>Serve per descrivere come appaiono gli elementi HTML.


## Come si collega il CSS all’HTML?
Hai 3 modi:


### Inline (dentro il tag)

```html
<p style="color: red;">Testo rosso</p>
```

### Interno al tag `<style>`
```html
<style>
  p { color: blue; }
</style>
```

### Esterno (in un file .css separato)
```html
<link rel="stylesheet" href="stile.css">
```

## Concetto da tenere a mente: il box model

Il box model è uno dei concetti fondamentali del CSS.
Ogni elemento HTML in una pagina web viene rappresentato come una scatola rettangolare.
Il box model spiega come viene calcolato lo spazio occupato da quella scatola.

```
┌─────────────────────────────────────┐
│             margin                 │
│ ┌───────────────────────────────┐  │
│ │           border              │  │
│ │ ┌───────────────────────────┐│  │
│ │ │         padding           ││  │
│ │ │ ┌───────────────────────┐ ││  │
│ │ │ │       content         │ ││  │
│ │ │ └───────────────────────┘ ││  │
│ │ └───────────────────────────┘│  │
│ └───────────────────────────────┘  │
└─────────────────────────────────────┘
```

### Content 
Il contenuto reale (testo, immagine, ecc.).
Proprietà: `width`, `height`

### Padding 
Lo spazio dentro il bordo, attorno al contenuto.
Es.: spazio tra il testo e il bordo di un pulsante.
Proprietà: `padding`, `padding-top`, `padding-left` ecc.

### Border 
Il bordo intorno all’elemento.
Proprietà: `border`, `border-width`, `border-color`, `border-radius`

### Margin 
Lo spazio esterno tra l’elemento e gli altri elementi vicini.
Proprietà: `margin`, `margin-top`, `margin-right` ecc.

> [!TIP]
> Di default, il width si riferisce solo al content.
> Se vuoi che width includa anche padding e border, puoi usare:
>```
>box-sizing: border-box;
>```

