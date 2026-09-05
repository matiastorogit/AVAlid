# AVAlid
Sistema que optimiza el proceso de contratación al automatizar la validación de documentos laborales mediante inteligencia artificial y OCR.

---
Nota: El repositorio original de este proyecto se mantiene privado por razones legales y de confidencialidad, ya que el software y su propiedad intelectual pertenecen a la empresa AVA Montajes Industriales, para la cual fue desarrollado.
---

AVALID — Sistema de Validación Automatizada de Documentos
Rol: Product Owner y Gestión de Proyecto
Cliente: AVA Montajes Industriales

Descripción General
Plataforma web diseñada para digitalizar y automatizar el proceso de contratación corporativo mediante la recepción y validación de documentos laborales. Integra un motor de Inteligencia Artificial y OCR para extraer información clave, realizar validaciones cruzadas en tiempo real y entregar al equipo de Recursos Humanos un sistema de trazabilidad completa por cada expediente.

Arquitectura y Funcionalidades Clave

Diseño e integración de un pipeline de análisis documental asíncrono de 8 etapas, incluyendo extracción de texto (Tesseract, EasyOCR), clasificación de documentos (TF-IDF, Reglas lógicas) y validación cruzada con datos de entrada.

Arquitectura basada en microservicios, comunicando el sistema central estructurado en Laravel con un servicio de análisis en Python (FastAPI).

Implementación de un sistema de colas (Queue) para el procesamiento en segundo plano de tareas de alto consumo y para el envío de invitaciones masivas utilizando la API nativa de Gmail.

Modelado de bases de datos relacionales multi-schema en PostgreSQL y desarrollo de un sistema de control de acceso basado en roles (SuperAdministrador, Administrador, RRHH, Reclutador).

Gestión técnica y documental del proyecto, elaborando las Especificaciones de Requisitos de Software (SRS) y orquestando el ciclo de desarrollo del equipo bajo metodologías ágiles.

Stack Tecnológico

Backend: Laravel 13.3, PHP 8.3, PostgreSQL, Laravel Queue.

Frontend: React 19, TypeScript 5.7, Inertia.js 2, Tailwind CSS 4.

Microservicio IA: Python 3.11, FastAPI, Tesseract OCR, EasyOCR, Scikit-learn, pdfplumber.

Infraestructura: Docker, Nginx, Redis.
