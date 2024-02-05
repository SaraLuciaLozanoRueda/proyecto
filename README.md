# 1

```
git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold
red)%h%C(reset) - %C(bold green) (%ar)%C(reset)%C(white)%s%C(reset)%C(dim
white)-%an%C(reset)%C(bold yellow)%d%C(reset)' --all"
```



- #### **git config --global:** es la propiedad que indica que se realizara un cambio global en el git.

- **alias.lg:** establece un alias o nickname.

- **--graph:** represesentacion grafica del historial.

- **--abbrev-commit:** muestra el hash (numero de identificacion del commit) del commit abrevidado.

- -**-decorate:** muestran las referencias junto a los commits.

- **--format=format:** define una personalizacion para los datos de salida.



| '%C(bold red)%h%C(reset)            | hash abreviado en rojo y negrita             |
| ----------------------------------- | -------------------------------------------- |
| **- %C(bold green) (%ar)%C(reset)** | fechas en negrita y verde                    |
| **%C(white)%s%C(reset)**            | mensaje del commit en blanco                 |
| **%C(dim white)-%an%C(reset)**      | nombre del autor en blanco y poca intensidad |
| **%C(bold yellow)%d%C(reset)'**     | referencias en amarillo y negrita            |

# 2

#### git config --global alias.l-1 "log -1 HEAD"

- `alias.l-1`: Estoy creando  un alias llamado "l-1".
- `"log -1 HEAD"`: Este es el comando real que se ejecutará cuando uso  el alias "l-1". Está diciendo a Git que muestre el historial de commits (`log`) limitado a un solo commit (`-1`) desde la rama actual (`HEAD`).

# 3

#### git config --global alias.ec 'config --global --edit'

- ec.: quiere decir que estoy poniendo un alias llamado "ec" para editarlo mas facil

  

​	con la funcion dada en la diapositiva sucede lo siguiente:

1. **git config --global core.editor ‘code --wait’**

   En esta línea de comando, estás configurando el editor por defecto que Git usará para abrir mensajes de commit, archivos de configuración, etc. En este caso, el editor configurado es Visual Studio Code, representado por el comando `code --wait`. La opción '--wait' significa que Git esperará a que cierres el editor antes de continuar con la ejecución del siguiente comando. Esta configuración es útil para asegurarse de que Git no continúe hasta que hayas completado tu mensaje de commit u otras operaciones de edición.

# 4

```
 git config --global alias.ultimo "log --graph --abbrev-commit --decorate --format=format'%C(bold
emphasis purple)%h%C(reset) %C(dim
white)-%an%C(reset)%C(strike blue)%d%C(reset)' --all"
```

git config --global alias.ultimo: Estoy configurando un alias global llamado "ultimo".

**log --graph --abbrev-commit --decorate --format=format'...' --all:** Especifica que estás utilizando el comando git log con varias opciones para obtener un historial de commits más detallado y de todos los branches (--all).

**%C(bold emphasis purple)%h%C(reset):** Muestra el hash del commit en color morado y negrita.
**%C(dim white)-%an%C(reset):** Muestra el nombre del autor precedido por un guion en color blanco atenuado o gris claro.
**%C(strike blue)%d%C(reset):** Muestra las ramas y etiquetas del commit en azul con un efecto de tachado.