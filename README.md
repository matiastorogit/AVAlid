# AVAlid
Sistema que optimiza el proceso de contratación al automatizar la validación de documentos laborales mediante inteligencia artificial y OCR.

---
Nota: El repositorio original de este proyecto se mantiene privado por razones legales y de confidencialidad, ya que el software y su propiedad intelectual pertenecen a la empresa AVA Montajes Industriales, para la cual fue desarrollado.
---

### AVALID — Sistema de Validación Automatizada de Documentos

Plataforma web diseñada para digitalizar y automatizar el proceso de contratación corporativo mediante la recepción y validación de documentos laborales. Integra un motor de Inteligencia Artificial y OCR para extraer información clave, realizar validaciones cruzadas en tiempo real y entregar al equipo de Recursos Humanos un sistema de trazabilidad completa por cada expediente.

# Arquitectura y Funcionalidades Clave

- Diseño e integración de un pipeline de análisis documental asíncrono de 8 etapas, incluyendo extracción de texto (Tesseract, EasyOCR), clasificación de documentos (TF-IDF, Reglas lógicas) y validación cruzada con datos de entrada.

- Arquitectura basada en microservicios, comunicando el sistema central estructurado en Laravel con un servicio de análisis en Python (FastAPI).

- Implementación de un sistema de colas (Queue) para el procesamiento en segundo plano de tareas de alto consumo y para el envío de invitaciones masivas utilizando la API nativa de Gmail.

- Modelado de bases de datos relacionales multi-schema en PostgreSQL y desarrollo de un sistema de control de acceso basado en roles (SuperAdministrador, Administrador, RRHH, Reclutador).

- Gestión técnica y documental del proyecto, elaborando las Especificaciones de Requisitos de Software (SRS) y orquestando el ciclo de desarrollo del equipo bajo metodologías ágiles.

# Stack Tecnológico

- Backend: Laravel 13.3, PHP 8.3, PostgreSQL, Laravel Queue.

- Frontend: React 19, TypeScript 5.7, Inertia.js 2, Tailwind CSS 4.

- Microservicio IA: Python 3.11, FastAPI, Tesseract OCR, EasyOCR, Scikit-learn, pdfplumber.

- Infraestructura: Docker, Nginx, Redis.

## Flujo de trabajo anterior - Extracto de presentación de sprint final AVA
<img width="1172" height="655" alt="image" src="https://github.com/user-attachments/assets/993eb9d5-2ef0-4db9-bb7c-d2f8bc645d71" />
<img width="1155" height="555" alt="image" src="https://github.com/user-attachments/assets/b806ef93-12bd-4d38-940e-5edd330abb5a" />

## AVALID - Extracto de presentación de sprint final AVA
<img width="1173" height="640" alt="image" src="https://github.com/user-attachments/assets/805326ac-24fb-41df-8952-a508c14dbd33" />

## Ficha de información postulante - Portal de postulación (Destinado a cargos de obra y administrativos)
<img width="1280" height="720" alt="ezgif-6d87db77bb49c13d" src="https://github.com/user-attachments/assets/5cc441d7-5bc9-484c-8ce8-592260456dd1" />
<img width="1280" height="720" alt="ezgif-6eac2730a2825de6" src="https://github.com/user-attachments/assets/8a5347c8-01bd-4029-9e53-e5c09402f97b" />

## Subida de documentos - Portal de postulación (Destinado a cargos de obra y administrativos)
<img width="1280" height="720" alt="subidadocs1" src="https://github.com/user-attachments/assets/67704ffb-5a26-48be-aa1f-27cd064661ef" />

## Login trabajadores AVA - Portal de recursos humanos
<img width="1280" height="720" alt="loginadmin" src="https://github.com/user-attachments/assets/129a4f49-69ea-4ae4-8d33-ef86e3ecb8d0" />

## KPIs - Portal de recursos humanos
<img width="1280" height="720" alt="ezgif-68e76b5917741491" src="https://github.com/user-attachments/assets/11a73c2f-ddb1-4ad5-b567-5a506b4a142b" />
<img width="1151" height="584" alt="image" src="https://github.com/user-attachments/assets/faf95d81-fae4-40bf-b9d2-b08489fc7a06" />

## Gestión de postulantes - Portal de recursos humanos
<img width="1280" height="720" alt="ezgif-6d8ab9a5583e6b59" src="https://github.com/user-attachments/assets/7ae186ef-e75e-430e-9028-bc8f65a5625a" />


## Gestión de faenas - Portal de recursos humanos
<img width="1280" height="720" alt="vistaadmin4verfaenas" src="https://github.com/user-attachments/assets/1edcb218-1220-4c7a-bf62-35899fd53b25" />
<img width="1280" height="720" alt="vistaadmin5editfaena" src="https://github.com/user-attachments/assets/1a8f60a4-60f7-478e-be16-3153d4bf5e6b" />
<img width="1280" height="720" alt="vistaadminverfaenas2" src="https://github.com/user-attachments/assets/368ccc1c-85e2-45d1-bea8-e89696775f7c" />

## Seguimienmto de emails - Portal de recursos humanos
# Las postulaciones podían enviarse via correo. Se hacía seguimiento de [correo enviado, link abierto, postulación enviada, estado del candidato]
<img width="1167" height="288" alt="image" src="https://github.com/user-attachments/assets/97434ac2-9d88-46e8-84d4-052eae92e4a7" />

## Arquitectura de microservicios y eventos del sistema
<img width="3492" height="2261" alt="AVALID_arquitectura_sistema" src="https://github.com/user-attachments/assets/0af12948-8d01-42b4-a6b8-3713aedc82a7" />




