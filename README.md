# iRedAdmin-Pro-SQL

### Repositorio gratuito & de código abierto de iRedAdmin-Pro-SQL

Esta es una carga gratuita del último paquete "iRedAdmin-Pro-SQL" (5.4).  Espero que algunas personas encuentren esto útil.  Estuve buscando durante bastante tiempo en línea pero no pude encontrar una copia distribuida gratuitamente, a pesar de que técnicamente la licencia no te impide compartirla, como menciono a continuación.

Como nadie más lo hizo, ahora lo haré yo.  Las pocas modificaciones realizadas se enumeran a continuación.  ¡Agradéceme después! <br><br>

-----
<details>
  <summary>Legal mumbo-jumbo</summary>

  ### yoUrE brEAkInG tHE liCeNsE...

  ```console
  El cliente NO tiene permitido redistribuir o revender iRedAdmin-Pro (...) como su propio producto. 
  ```
  aka. Se me permite redistribuir iRedAdmin-Pro, reconociendo que es su código, lo cual hago por la presente.  No reclamo que esto sea mi propio producto, es su creación, no la mía.  Simplemente lo reflejo y lo mantengo aquí, como lo hago:
  1. Necesita control de versiones, etc..
  2. Me gusta modificar cosas que tengo y vincularlas a 1. No quiero volver a hacer mis cambios después de cada actualización.
  3. No estoy de acuerdo con el hecho de que se supone que debes pagar por un código fuente legible por humanos.
  4. No estoy legalmente autorizado a hacerlo, según el acuerdo que acepté en el momento de la compra.
  
  ### ... aND thE nEw EulA

  Nuevamente incorrecto.  De ninguna manera me dicen que lo acepte.  Además, el EULA no cambia el pasado.  Esta es una copia modificada y de código abierto del producto durante una época en la que estaba bien.  Ahora, el nuevo EULA *en teoría* solucionaría esto para mí.  **SIN EMBARGO**, no tengo que aceptarlo para descargar la actualización, no tengo que aceptarlo para instalar la actualización y no se me pide que lo acepte antes de su uso.  De hecho, si git no me lo hubiera dicho, ni siquiera lo sabría.  Dicho esto, es posible que el EULA no exista.  Al menos ese es su estatus legal actual.  Este pobre "por favor lea" en el archivo Léame que nadie lee tampoco ayuda.  ¿Te pide que lo leas, pero nunca que lo aceptes o lo entiendas?  Dios, la jerga legal de algunas personas es terriblemente mala.<br><br>

  ### Qué tal si te hago uno mejor
  Dado que a este proyecto le faltaba algún tipo de protección legal adecuada, podría arruinar totalmente el día del autor, pero no lo haré.  Sin embargo, lo que haré será *agregar* basura legal, así que ya.  Eche un vistazo a la licencia adjunta a este proyecto.

</details>

-----

Sólo se cambiaron muy pocos archivos.  El archivo original ha sido comentado para que puedas entender lo que hacía antes.

```console
- libs/sysinfo.py
# This script did the actual check
# Este script hizo la verificación real.
  
- templates/default/panel/license.html
# Tiny change to remove the "Renew License" button
# Pequeño cambio para eliminar el botón "Renovar licencia"
  
- static/default/css/screen.css
# ctrl+shift+I formatting & changed color from green to purple.
# ctrl+shift+I formato y cambio de color de verde a morado
# CSS file looks disgusting, refusing to clean that
# El archivo CSS se ve desagradable y se niega a limpiarlo.
```

Eso es todo <br><br>

-----

### Algunos enlaces útiles:

 - Si ya tiene instalado iRedAdmin o una versión anterior de iRedAdmin-Pro, siga [el tutorial de actualización](https://docs.iredmail.org/migrate.or.upgrade.iredadmin.html) para obtener lo último iRedAdmin-Pro.

- [Notas de lanzamiento](https://docs.iredmail.org/iredadmin-pro.releases.html)

- [iRedAdmin-Pro documentaciones](https://docs.iredmail.org/#iredadmin)<br><br>

-----

### Detalles originales

|Característica	                           | iRedAdmin (OSE) | iRedAdmin-Pro|
|------------------------------------------|-----------------|--------------|
$\textcolor{orange}{\textsf{Localized Web Interface}}$<br>English, German, Spanish, French, Italian, Polish, Chinese, and more.	           |     X           |    X         |
$\textcolor{orange}{\textsf{RESTful API Interface}}$<br>Lea nuestro [API documentation](https://docs.iredmail.org/iredadmin-pro.restful.api.html) | | X |
$\textcolor{orange}{\textsf{Unlimited Mail Domains}}$<br>Aloja tantos dominios de correo como quieras | X | X |
$\textcolor{orange}{\textsf{Unlimited Mail Users}}$<br>Con control de cuota de buzón por usuario | X | X |
$\textcolor{orange}{\textsf{Unlimited Mailing List/Aliases}}$<br>Administrar miembros, políticas de acceso. | | X |
$\textcolor{orange}{\textsf{Unlimited Domain-Level Admins}}$<br>Ascienda a un usuario de correo a la función de administrador de dominio o cree una cuenta de administrador de dominio separada		| | X |
$\textcolor{orange}{\textsf{Advanced Domain Management}}$<br>Cuota de buzones de correo a nivel de dominio, número límite de cuentas de usuario/lista/alias, retransmisión, BCC, alias, dominio, general, Backup MX, limitación, listas grises, listas blancas, listas negras, política de spam, longitud de la contraseña del usuario y control de complejidad		| | X |
$\textcolor{orange}{\textsf{Advanced User Management}}$<br>CCO por usuario, retransmisión, reenvío de correo, direcciones de alias, limitación, listas grises, listas blancas, listas negras, política de spam, restricción de IP/red de inicio de sesión, cambio de dirección de correo electrónico		| | X |
$\textcolor{orange}{\textsf{Self-Service}}$<br>Permitir al usuario final administrar sus propias preferencias: Contraseña, Reenvío de correo, Listas blancas, Listas negras, Correos en cuarentena, Política de spam		| | X |
$\textcolor{orange}{\textsf{Service Control}}$<br>Un clic para habilitar/deshabilitar los servicios de correo para el usuario de correo: POP3, IMAP, SMTP, filtro Sieve, reenvío de correo, BCC y más.		| | X |
$\textcolor{orange}{\textsf{Spam/Virus Quarantining}}$<br>Poner en cuarentena SPAM/Virus detectados en la base de datos SQL PostgreSQL para su posterior administración (eliminar, publicar, incluir en la lista blanca, lista negra)		| | X |
$\textcolor{orange}{\textsf{View basic info of all sent and received emails}}$<br>Remitente, Destinatario, Asunto, Puntuación de spam, Tamaño, Fecha | | X |
$\textcolor{orange}{\textsf{Throttling}}$<br>Basado en: tamaño máximo de un solo correo electrónico, número máximo de correos electrónicos entrantes/salientes, tamaño acumulado de todos los correos electrónicos entrantes/salientes		| | X |
$\textcolor{orange}{\textsf{Whitelisting, Blacklisting}}$<br>Basado en: direcciones IP/redes, dirección del remitente, nombre de dominio del remitente | | X |
$\textcolor{orange}{\textsf{Searching Account}}$<br>Búsqueda con nombre para mostrar o dirección de correo electrónico, nombre de dominio | | X |
$\textcolor{orange}{\textsf{Log Maildir Path of Deleted Dail User}}$<br>Puede eliminar el buzón del sistema de archivos más adelante, ya sea manualmente o con un trabajo cron		| | X |
$\textcolor{orange}{\textsf{Log Admin Activities}}$<br>Creación, activación, eliminación de cuenta, cambio de contraseña y más.. | | X |
$\textcolor{orange}{\textsf{Fail2ban Integration}}$<br>Vea información de la dirección IP prohibida (país/ciudad, nombre DNS inverso), registre las líneas que activaron la prohibición (es fácil solucionar el motivo de la prohibición) y desbanquéela con un solo clic.		| | X |
$\textcolor{orange}{\textsf{Last login track}}$<br>Ver la hora del último inicio de sesión del usuario a través de los servicios IMAP y POP3, también la hora del último correo electrónico entregado (localmente)		| | X |
$\textcolor{orange}{\textsf{Export all managed mail accounts}}$| | X |
$\textcolor{orange}{\textsf{Export statistics of admins}}$| | X |

<br><br>

-----

### My wallet is crying now. Please give this repo a star to cheer me up

![2023-04-10-064957](https://user-images.githubusercontent.com/104512346/230828290-cf3aec7c-a850-494a-94f9-0f739ffc6b48.png)

----- 
<p align="center"><a href="https://free-tools.club/discord">Join the Discord and help us!</a></p>
