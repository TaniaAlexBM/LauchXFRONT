# Requerimientos
<table>
  <tr>
    <td><img src = "./IMG/logo.png" width = "150" height = "150" alt = "Logo AbogaBot"/></td>
    <td><h1><strong>Proyecto AbogaBot<strong></h1></td>
  </tr>
</table>


## 1. Descripción general del requerimiento

| PROYECTO                                                                 | AbogaBOT                         |
| ------------------------------------------------------------------------ | -------------------------------- |
| Nombre Requerimiento:                                                    | Aplicación web                   |
| Fecha Solicitud:                                                         | 18/02/2022                       |
| Responsable(s) Solicitud:                                                | Juan Rodrigo Martínez Plascencia |
| Dependencia(s) Solicitante:                                              | Frontend                         |
| Responsable Funcional designado por el equipo de desarrollo de software: | Tania Alejandra Benítez Martínez |


## 2. Fase de formalización

### Descripción de la solicitud
<table>
    <thead>
        <tr>
         <th>Usuario solicitante</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><p>Es un despacho de abogados que quiere automatizar las demandas de sus clientes, esto lo harán a través de una página web llenando un formulario.</p>
            <p>Al momento de llenar el formulario se manda al proceso de pago para finalizar la transacción. 
            Para dar seguimiento a su demanda, el cliente crea una cuenta en la plataforma y verá el seguimiento de cada una de las actualizaciones del proceso legal.</p>
            <p>El administrador del sitio recibe la notificación de una nueva demanda y con los datos llenados del formulario se crea automáticamente el documento legal en formato word para empezar el proceso.</p>
            <p>El administrador recibe el pago y debe de ser capaz de verlo en un dashboard para ver la cantidad de ingresos recibidos.</p>
            <p>El administrador actualiza el proceso de la demanda y agrega comentarios en cada paso del proceso.</p>
            <p>Al usuario le llegan correos de notificación para saber el avance de su proceso.</p>
            <p>La página debe de ser responsive para poderla ver desde el celular.</p>
            <p>La preferencia de colores del cliente es azul marino y blanco, pero acepta propuestas.</p></td>
        </tr>
    </tbody>
</table>
<table>
    <thead>
        <tr>
         <th>Líder funcional</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>La aplicación web automatizará la petición, registro y creación del documento inicial de la demanda que el usuario solicite al despacho. También los pagos y actualizaciones serán mediante la misma.
            Será una página web que se podrá utilizar en cualquier dispositivo, en donde encontrarás:
            <ul>
                <li>Formulario de registro</li>
                <li>Proceso de pago</li>
                <li>Documento inicial de la demanda generado automáticamente</li>
                <li>Perfil del cliente</li>
                <li>Perfil del administrador</li>
                <li>Seguimiento de demandas</li>
                <li>Dashboard para el administrador</li>
                <li>Contacto con el administrador</li>
            </ul>
            El administrador de la página web recibirá notificaciones vía correo electrónico por:
            <ul>
                <li>Registro de nueva demanda</li>
                <li>Pagos por servicios</li>
            </ul>
            además, podrá actualizar la demanda y dejar comentarios en cada paso del proceso.
            El cliente, recibirá un correo electrónico avisándole:
            <ul>
                <li>Actualizaciones hechas por el administrador</li>
                <li>Avance de la demandas</li>
            </ul>
            también, podrá ver los avances de su demanda en el dashboard de su perfil.
            <p>La apariencia de la página se prefiere azul marino con blanco, pero está abierto a propuestas.</p></td>
        </tr>
    </tbody>
</table>


## 3. Análisis de requisitos y requerimientos
| Fecha de inicio | Fecha final |
| ---- | ---- |
| 18/02/2022 | 25/02/2022 |

| Términos de Referencia | |
| ----- | ----- |
| Alcance de la solución |<ul><li>Maquetación UX/UI</li><li>Diseño de las vistas del frontend</li><li>Diseño de la Base de Datos</li><li>Diseño de los endpoints necesarios</li><li>Conectar frontend con backend</li><li>Desplegar la aplicación web</li><li>La aplicación web será responsiva</li><li>Generar una demanda preliminar con los datos que el usuario ingrese</li><li>No se creará una aplicación móvil</li></ul> |
| Requerimientos Funcionales y criterios de aceptación | <ul><li>Registro del administrador</li><li>Registro de usuarios</li><li>Form para la información de la demanda</li><li>Generación del documento preliminar</li><li>Guardar, modificar y eliminar información de la demanda</li><li>Notificaciones vía correo electrónico para el administrador y para los usuarios</li></ul> |
| Requerimientos no Funcionales y de calidad | <ul><li>Utilizar azul marino y blanco</li><li>SEO</li></ul> |
| Precondiciones | <ul><li>Elección de servicio Cloud a utilizar</li><li>Restricciones de tecnologías</li><li>Presupuesto</li><li>Alcances de la aplicación</li><li>Escalabilidad</li></ul> |
| Requisitos técnicos | <table><thead><tr><th>Tipo de desarrollo</th><th>Base de Datos</th><th>Lenguajes</th></tr></thead><tbody><tr><td>Aplicación web</td><td>MySQL</td><td>JavaScript Java</td></tr></tbody></table> |
| Viabilidad técnica | Viable |


## 4.Levantamiento del requerimiento detallado

| Historia de usuario | Número 1  |
| ----- | ----- |
| Título | Registro en la aplicación web |
| Estimación | XL |
| Característica/Funcionalidad | El administrador y los usuarios podrán registrarse en la plataforma mediante un formulario que saldrá como opción en la página del login |
| Razón/Resultado | <ul><li>Registrar al administrador para que maneje el sistema</li><li>Registrar a los usuarios para que inicien el contrato del servicio</li></ul> |

| Historia de usuario | Número 2  |
| ----- | ----- |
| Título | Login de ususarios |
| Estimación | XL |
| Característica/Funcionalidad | Todos los usuarios podr acceder a los servicios de la aplicación siempre que estén registrados y puedan hacer login con su correo electrónico y contraseña |
| Razón/Resultado | <ul><li>Mostrar vista de login</li><li>Formulario de ingreso de correo electrónico y contraseña</li><li>Ingresar a su perfil si los datos que ingresó fueron los correctos</li></ul> |

| Historia de usuario | Número 3  |
| ----- | ----- |
| Título | Dashboard: Administrador |
| Estimación | L |
| Característica/Funcionalidad | El administrador entrará a un dashboard donde pueda ver los usuarios nuevos, estatus de todos los usuarios, cambios en las demandas y  |
| Razón/Resultado | <ul><li>Mostrar vista de perfil</li><li>Mostrar lista de nuevos usuarios en un lapso de tiempo</li><li>Mostrar actualizaciones hechas</li><li>Mostrar status de las demandas activas</li><li>Mostrar nuevos pagos</li></ul> |