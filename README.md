<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" /></a>
</p>

<h1 align="center">Servicio de Estudiantes y Apoderados - Sistema Escolar</h1>

## 📝 Descripción

Este repositorio contiene el código fuente del **Servicio de Estudiantes y Apoderados**. Este microservicio, desarrollado con **[NestJS](https://nestjs.com)**, está diseñado para que los estudiantes y sus apoderados puedan consultar de forma segura y sencilla toda su información académica relevante.

El propósito principal de este servicio es de **consulta (lectura)**. Sus responsabilidades incluyen:
-   **Consulta de Calificaciones:** Proveer acceso detallado a las notas y promedios obtenidos en las distintas asignaturas.
-   **Visualización de Asistencia:** Mostrar el registro histórico de asistencias, incluyendo ausencias, presencias y tardanzas.
-   **Acceso a Observaciones:** Permitir que los estudiantes y apoderados vean las observaciones (positivas, negativas o informativas) registradas por los docentes.
-   **Perfil Académico:** Exponer los datos generales del perfil del estudiante, como su curso y horario.

---

## 🔐 Autorización y Seguridad

La seguridad es primordial en este servicio. La lógica de negocio se asegura de que un usuario autenticado (estudiante o apoderado) **solo pueda acceder a su propia información o a la de sus pupilos**, validando en cada solicitud la correspondencia entre el ID del token JWT y el recurso solicitado.

---

## 🛠️ Tecnologías Utilizadas

-   **Framework:** [NestJS](https://nestjs.com/)
-   **Lenguaje:** [TypeScript](https://www.typescriptlang.org/)

---
## ▶️ Ejecutando la Aplicación

```bash
# Modo desarrollo con recarga automática
$ pnpm run start:dev

# Modo producción
$ pnpm run start:prod
