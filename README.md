##VIM

Interestin link

[Venture Into Vim](https://code.tutsplus.com/courses/venture-into-vim)

[Venturing into Vim - Screencast 1](https://code.tutsplus.com/tutorials/venturing-into-vim--net-15086)

[Oficial Page](http://www.vim.org/)

##Some Tip

Copy to clipboard, example:  `pwd | pbcopy`

Example:

```
$ curl -L "http://google.cl" | pbcopy
$ ps aux | pbcopy
$ ps aux | grep root | pbcopy
```

Paste from clipboar, example:  `pwd | pbpaste`

Example:

```
$ pbpaste | less
$ pbpaste > pastetest.txt
$ pbpaste | grep rcp
```
💡 Para ir a una letra en particular escribir:

```
f<letter> Example $fs
vf<letter> Example $vfs
```
💡 Para ir al inicio de una linea: cero

```
0
```
💡 Para seleccionar toda una palabra

```
viw // visual into word
```
💡 Para seleccionar toda una palabra, pero incluye el espacio en blanco

```
vaw // visual around word
```
💡 Para borrar una palabra seleccionada, funciona tanto la `x` como la `d`

💡 Para borrar una palabra seleccionandola al mismo tiempo, funciona tanto la `diw`, `daw`

💡 Hay una sutil diferencia cuando se usa comandos con palabras mayuscular y minusculas: `viw`, `viW` y `vaw` y `vaW`. Cual es la sutil diferencia?

💡 Podriamos copiar al clipboard usando estas notaciones: `yiw`, `yiw`, `yaw`, `yaw` y luego pegarlas con el comando `p`

##Paragraph

💡 El patron de `inner` o `all` `word` funciona para lo parrafos tambien:

```
vip // visual into pharagraph
vap // visual around pharagraph

```

##Sentences

💡 En el caso de sentencias este comando `gUis`  (g Uppercase inside sentence) convierte la sentecia en mayusculas

💡 En el caso de sentencias para borar tenemos este comando `das`  (delete around sentec sentence)

💡 En el caso de palabras que estan dentro de un tag  `vit`  (visual inside tag)

```
<body>This is the body of web page</body>
```

💡 En el caso de palabras que estan dentro de un tag  `vat`  (visual around tag) para seleccionar con todo el tag

💡 En el caso de palabras que estan dentro de un tag podemos cambiar lo que esta dentro usando este comando  `cit`  (change inside tag).

💡 En el caso de palabras que estan dentro parentesis podemos usar el mismo patron `vi(`, `vi)`  (visual inside simboloParentesis).

💡 En el caso de palabras que estan alrededor parentesis podemos usar el mismo patron `va(`, `va)`  (visual around simboloParentesis).

💡 En el caso de palabras que queremos cambiar que estan dentro parentesis podemos usar el mismo patron `ci(`, `ci)`  (change inside simboloParentesis).

💡 Lo mismo que para el parentesis funciona para las llaves: 

```
vi{  // visual inside {
vi}  // visual inside }
va{  // visual around {
va}  // visual around }
ci{  // change inside {
ci}  // change inside }
ca{  // change around {
ca}  // change around {
```

💡 Lo mismo que para el cochetes funciona para las llaves: 

```
vi[  // visual inside [
vi]  // visual inside ]
va[  // visual around [
va]  // visual around ]
ci[  // change inside [
ci]  // change inside ]
ca[  // change around [
ca]  // change around ]
```

💡 Lo mismo que para las comillas funciona para las llaves: 

```
vi"  // visual inside "
vi"  // visual inside "
va"  // visual around "
va"  // visual around "
ci"  // change inside "
ci"  // change inside "
ca"  // change around "
ca"  // change around "
```

💡 `vib`(visual inside b es dentro de parentesis) = ( )

💡 `vab`(visual around parentesis)

💡 `viB`(visual inside B es dentro de Llaves) = { }
💡 `vaB`(visual around B es dentro de Llaves) = { }

