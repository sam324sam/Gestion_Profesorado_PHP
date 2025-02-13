![Estado](https://img.shields.io/badge/Estado-En%20proceso-yellow?style=plastic)

# Inscripción a Cursos de Formación para Profesorado

## Descripción
Este proyecto es una aplicación web desarrollada en PHP que permite gestionar la inscripción de profesores a cursos de formación. La asignación de plazas se realiza de manera automatizada según los méritos de cada solicitante una vez finalizado el plazo de inscripción.

## Tecnologías Utilizadas
- **PHP** para la lógica del servidor.
- **MySQL** como sistema de gestión de base de datos.
- **HTML, CSS y JavaScript** para la interfaz de usuario.
- **Librerias PHP** uso de PHP-Mailer y FPDF
- **Servidor de correos** Uso del servidor Axigen de manera local

## Base de Datos
La aplicación utiliza una base de datos llamada `cursoscp` con las siguientes tablas:

<div align="center">
  <img src="imgGithub/GestionProfesoradoPHPDB.PNG" alt="Base de datos" width="500">
</div>

La cual puedes importar del archivo Import DB/cursos.sql

## Funcionalidades
- **Autenticación de usuarios**.

<div align="center">
  <img src="imgGithub/GestionProfesoradoPHPLogin.PNG" alt="Inscripcion" width="500">
</div>

- **Activar/Desactivar cursos** (Administrador).

<div align="center">
  <img src="imgGithub/GestionProfesoradoPHPCerrarCursos.png" alt="Act/Desac" width="500">
</div>

- **Realizar inscripción en un curso**.

<div align="center">
  <img src="imgGithub/GestionProfesoradoPHPCursos.PNG" alt="Base de datos" width="500">
</div>

- **Baremación automática de solicitantes tras cierre de inscripción** (Administrador).

<div align="center">
  <img src="imgGithub/GestionProfesoradoPHPBaremacion.png" alt="Baremacion" width="500">
</div>
  
- **Listar admitidos en un curso** (Administrador).

<div align="center">
  <img src="imgGithub/GestionProfesoradoPHPAdmitidos.png" alt="Admitidos" width="500">
</div>

- **Añadir/Eliminar cursos** (Administrador).

<div align="center">
  <img src="imgGithub/GestionProfesoradoPHPEliminar.png" alt="Eliminar cursos" width="500" height="200">
  <img src="imgGithub/GestionProfesoradoPHPCrear.png" alt="Añadir cursos" width="500" height="200">
</div>

- **Creacion de pdf para correo de notificacion**.

<div align="center">
  <img src="imgGithub/GestionProfesoradoPHPPDF.png" alt="Correo" width="500">
</div>


## Criterios de Baremación
La asignación de plazas se realiza según los siguientes méritos:

| Mérito | Puntos |
|--------|--------|
| Coordinador TIC | 3 |
| Grupo relacionado con las TICs | 3 |
| Programa bilingüe | 3 |
| Cargo de director | 1 |
| Cargo de Jefe de Estudios | 1 |
| Cargo de Secretario | 1 |
| Cargo de Jefe de Departamento | 1 |
| Antigüedad | 15 |
| Profesor en activo | 3 |

## Instalación y Configuración
1. Clonar este repositorio:
   ```bash
   git clone https://github.com/sam324sam/inscripcion-cursos.git
   ```
2. Configurar el servidor web con PHP y MySQL.
3. Importar la base de datos desde `cursoscp.sql`.
4. Configurar las credenciales de la base de datos en `db.php`.
5. Descargar la librería de **PHP Mailer**: [PHPMailer en GitHub](https://github.com/PHPMailer/PHPMailer).
6. Descargar la librería **Fpdf186 v1.86**: [FPDF](http://www.fpdf.org/).
7. Coloque las librerias en la carpeta 'librerias' del proyecto.
8. Instalacion de un servidor mail En este caso El servidor Axigen [Axigen](https://www.axigen.com/mail-server/download/).
9. Ejecutar la aplicación desde el navegador.


## Nota
Si quiere realizar cambios en el PDF o en el encvio del correo esto se encuentra en funciones_admin/funciones_db.php en las dos ultimas funciones.
El PDF no admite caracteres especiales. Si deseas aportar una solución, puedes hacerlo mediante un [pull request](https://github.com/sam324sam/Gestion_Profesorado_PHP/pulls) o dejando un comentario en la sección de **Issues** de este repositorio.

Agradesco cualquier contribución que ayude a mejorar el proyecto.

## Autor
Este proyecto ha sido desarrollado por Samuel Moniz Pereira.

## Licencia
Este proyecto se distribuye bajo la licencia MIT.

## Contribuir al Proyecto
Para conocer cómo contribuir, revisa nuestras [pautas de contribución](https://github.com/sam324sam/sam324sam/blob/main/CONTRIBUTING.md).

