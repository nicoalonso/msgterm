# Descripción

Clase para mostrar mensajes en el terminal con diferentes estilos.

Se ayuda de la librería `termcolor` para mostrar los textos en color y con otros estilos.



## Características

Se pueden mostrar mensajes personalizados o usar los ya definidos en la clase:

* ***debug***: mostrar mensajes de depuración
* ***info***: mostrar información al usuario
* ***text***: mostrar textos
* ***success***: mostrar mensajes de éxito
* ***warning***: mostrar advertencias al usuario
* ***alert***: mostrar alertas al usuario
* ***error***: mostrar errores
* ***fatal***: mostrar errores fatales
* ***help***: mostrar mensajes de ayuda al usuario



Ejemplos:

```python
MsgTerm.verbosity(MsgTerm.DEBUG)  # Set level of verbosity
MsgTerm.message('Text messages')
MsgTerm.debug('debug')
MsgTerm.info('info')
MsgTerm.text('text')
MsgTerm.success('success')
MsgTerm.warning('warning')
MsgTerm.alert('alert')
MsgTerm.error('error')
MsgTerm.fatal('fatal')
MsgTerm.help('help')

# Print a list of messages in paragraph style
MsgTerm.message('Paragraph Style', label='#', bold=True, hr=True, type=MsgTerm.SUCCESS)
msgs = ['This is a message', 'that to show in multiple lines', 'like as a paragraph style']
MsgTerm.message(msgs, paragraph=True, label=' ', bold=True, type=MsgTerm.INFO)
```


Se puede definir el nivel de verbose que se quiere mostrar en pantalla:

```python
MsgTerm.verbosity(MsgTerm.ALERT)
```



## Dependencias

* `termcolor`

  Instalar

  ```bash
  pip install termcolor
  ```

  