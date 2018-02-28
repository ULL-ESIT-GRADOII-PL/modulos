# Ejemplo de solución a la práctica de publicar un módulo en npm

## Reto

Escriba un nuevo tipo de celda `ColorCell` que hace que la celda se muestre con el font en el color especificado

```js
[
  {"name": {"type": "ColorCell", "params": ["Teide", {"c": blue", "bg": "White"}]}, "height": 3718, "country": "Spain"},
  {"name": "Kilimanjaro\nMontaña mágica", "height": 5895, "country": "Tanzania"},
  {"name": "Everest", "height": 8848, "country": "Nepal\nPaís lejano"},
  {"name": {"type": "StrechCell", "params": ["Mount Fuji", 2]}, "height": 3776, "country": "Japan"},
  {"name": "Mont Blanc", "height": {"type": "ColorCell", "params": [4808, {"c": "red"}]}, "country": "Italy/France"},
  {"name": "Vaalserberg", "height": 323, "country": "Netherlands"},
  {"name": "Denali", "height": 6168, "country": "United States"},
  {"name": "Popocatepetl", "height": 5465, "country": { "type": "RCell", "params": ["Mexico"]} }
]
```

* Use el módulo [chalk](https://www.npmjs.com/package/chalk) para insertar los colores:

  ```js
  log(chalk.red('Hello', chalk.underline.bgBlue('world') + '!'));
  ```
  ANSI sequences were introduced in the 1970s to replace vendor-specific sequences and became widespread in the computer equipment market by the early 1980s. 
  Certain sequences of bytes, most starting with `Esc` and `[`, are embedded into the text, which the terminal looks for and interprets as commands, not as character codes.
* Publique el nuevo tipo de celda como un módulo npm `@aluXXX/mimodulo-plugin-colorcell`
* Compruebe que la funcionalidad de su módulo queda extendida correctamente con el módulo plugin

