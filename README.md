# F1Bets
Proyecto final de DAW: donde uso angular con el framework de Ionic como front, y Google Firebase como back

## Descripción
  F1Bets es una plataforma de apuestas de Fórmula 1, en la que se puede ver listas de pilotos y circuitos de la F1, así como añadir, eliminar o editar elementos en la lista si se está registrado como administrador (mediante un botón en los ajustes se podrá cambiar a rol de administrador con motivo de testeo). También estará la pestaña de apuestas donde se almacenará y se podrá añadir apuestas a cada circuito del piloto ganador, en caso de acertar o no se ganará o perderá la cantidad correspondiente. Como ejemplo al registrarse se dará automáticamente un bono de 100€, ya que la app no funcionará con dinero real, será todo ficticio con fines de entretenimiento.

## Tutorial de uso y secciones de la app
  Las secciones con las que cuenta esta app son:

  - **Login y regsiter:**
  Página para iniciar sesión o registrarse en caso de no tener cuenta
  ![login](https://github.com/user-attachments/assets/101e3a6c-f555-422c-95eb-ed43c9bb73ad)
  ![register](https://github.com/user-attachments/assets/09bf0fee-d755-4386-b618-576302fca767)

  - **Home**
    La primera página que se ve al iniciar sesión, en la que se ve un slider presentando las funciones de la app y acceder a ellas mediantes los tabs de la barra inferior o al popover de usuario


  - **Ajustes**
    El popover que se menciona anteriormente permite que se pueda acceder a ajustes desde cualquier parte de la app, donde están las funciones de cerrar sesión, eliminar la cuenta y editar datos del usuario como el nombre de usuario


  - **Pilotos**
    La lista de pilotos, donde se puede hacer click en ellos para ver detalles y ajustes de los mismos, como eliminarlos o editarlos, además de añadir nuevos, en caso de estar registrado como admin.


  - **Circuitos**
    La lista de circuitos, que funciona igual que la lista de pilotos anteriormente mencionada, función de eliminar, editar, añadir y ver detalles


  - **Apuestas**
    La lista de apuestas en curso, donde se podrá añadir la apuesta que se quiera realizar en el circuito por el piloto con el dinero que se desee siempre que se tenga

## ¿Por qué usar Google Firebase en lugar de un backend tradicional?
  En este proyecto decidí usar Firebase como backend en lugar de una arquitectura tradicional basada en frameworks como Spring Boot con Java, por ejemplo, debido a su simplicidad y mayor velocidad de desarrollo. Firebase ofrece un Backend-as-a-service (BaaS) que elimina la necesidad de configurar y mantener un servidor propio.

### Ventajas de usar Firebase
  - **Infraestructura menos compleja**<br>
     Firebase proporciona servicios preconfigurados como autenticación, base de datos en tiempo real y Firestore, almacenamiento, funciones en la nube, etc., lo que permite centrarse más en la lógica de negocio y experiencia de usuario que en el mantenimiento de servidores y APIs REST tradicionales.
  - **Funciones en la nube (Cloud Functions)**<br>
     Permite ejecutar lógica del lado del servidor sin mantener un servidor. Esto cubre muchas necesidades típicas de un backend tradicional, como validaciones o integración con otros servicios.
  - **Desarrollo más rápido**<br>
    Al reducir la complicación de desarrollar un backend desde cero, te permite desarrollar las funcionalidades de la aplicación de forma más rápida y avanzada, pudiendo añadirle más funcionalidades, como las que mostraré en el siguiente apartado:

## Funcionalidades adicionales
  - **Ngx-translate**<br>
    Es una librería para Angular que me ha permitido añadir dos idiomas simultaneos en la aplicación, inglés y español, pudiendo cambiar entre ellos en cualquier momento desde un botón en la barra superior.
  - **Monedero**<br>
    La app cuenta con una función de monedero que te proporcionará con un bono ficticio de 100€ iniciales para apostar y que se reducirá o aumentará según las apuestas que se hagan.

## Advertencia
  Hay funciones como poder autoasignarse el rol de administrador, y con este mismo rol reiniciarse el monedero a 100€ que se puede hacer debido a que la aplicación se mantendrá en modo de prueba, para facilitar su prueba y presentación
