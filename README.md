##VIM

Interestin link

[Venture Into Vim](https://code.tutsplus.com/courses/venture-into-vim)

[Venturing into Vim - Screencast 1](https://code.tutsplus.com/tutorials/venturing-into-vim--net-15086)

[Oficial Page](http://www.vim.org/)

##Some Tip

Copy to clipboar, example:  `pwd | pbcopy`

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
viw // visual inter word
```
💡 Para seleccionar toda una palabra, pero incluye el espacio en blanco

```
vaw // visual all word
```
💡 Para borrar una palabra seleccionada, funciona tanto la `x` como la `d`

💡 Para borrar una palabra seleccionandola al mismo tiempo, funciona tanto la `diw`, `daw`

💡 Hay una sutil diferencia cuando se usa comandos con palabras mayuscular y minusculas: `viw`, `viW` y `vaw` y `vaW`

💡 Para borrar una palabra seleccionandola al mismo tiempo, funciona tanto la `diw`, `daw`

💡 Podriamos copiar al clipboard usando estas notaciones: `yiw`, `yiw`, `yaw`, `yaw` y luego pegarlas con el comando `p`








