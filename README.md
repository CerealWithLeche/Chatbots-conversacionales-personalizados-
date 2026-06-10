# Desarrollo de Chatbots Personalizados con la API de OpenAI
Este repositorio contiene un ecosistema modular para el desarrollo e integración de chatbots adaptativos y personalizados en sitios web. El sistema está diseñado para consumir los modelos de lenguaje de OpenAI mediante una arquitectura eficiente, asegurando respuestas dinámicas y un comportamiento alineado a los requerimientos específicos de cada entorno (institucional, comercial o académico).
Este ecosistema implementa una arquitectura desacoplada que permite transformar la temática del chatbot instantáneamente con solo cambiar el identificador del asistente en el backend, reutilizando el 100% de la infraestructura de interfaz y seguridad.

---

## Decisiones de Arquitectura y Seguridad (Production-Ready)

El proyecto está diseñado bajo el principio de separación de responsabilidades para garantizar la seguridad en entornos de hosting tradicionales:

* **Frontend Agnóstico:** Una interfaz de usuario limpia y responsiva construida en JavaScript nativo. No depende de frameworks pesados, lo que facilita su incrustación en cualquier sitio web existente.
* **Proxy Seguro en Backend (PHP):** Toda la comunicación con los endpoints de OpenAI se centraliza del lado del servidor. Esto encapsula por completo las API keys corporativas, evitando que los tokens de acceso queden expuestos en el navegador del cliente.
* **Control de Flujo Asíncrono:** Consumo eficiente de la API de Asistentes mediante ciclos de monitoreo activo (polling) y control de estados en tiempo real (indicadores de escritura, manejo de errores de red y detención inmediata de peticiones mediante AbortController).

---

## Características Técnicas Destacadas

* **Aislamiento de Credenciales:** Consumo seguro de APIs de Inteligencia Artificial sin exposición de llaves criptográficas en el cliente.
* **Renderizado Científico Integrado:** Soporte nativo para la visualización de ecuaciones y fórmulas matemáticas complejas mediante MathJax, ideal si el asistente se configura para entornos de ingeniería, finanzas o ciencia.
* **Formateo Enriquecido (Markdown):** Procesamiento dinámico de texto (listas, negritas, bloques de código y enlaces estructurados).
* **Utilidades de Experiencia de Usuario:** Sistema de notificaciones en pantalla (Toast) y función integrada para limpiar la sintaxis Markdown al copiar las respuestas al portapapeles.
* **Diseño UI/UX Ultra-Responsivo:** Interfaz moderna estilizada con variables CSS y media queries avanzadas, optimizada bajo el enfoque Mobile-First.

---

## Flexibilidad y Casos de Uso (Reciclable)

El Core del sistema es 100% parametrizable. Al modificar el identificador del asistente y las instrucciones del sistema en el panel de OpenAI, la plataforma se adapta inmediatamente a verticales como:

1. **Entornos Clínicos y Médicos:** Asistentes especializados para la atención de pacientes, filtrado de dudas frecuentes o soporte en consultorios.
2. **Áreas Académicas y de Investigación:** Soporte de tutorías, resolución de problemas con notación matemática y consulta de bases de conocimiento técnicas.
3. **Plataformas Institucionales y Comerciales:** Captación de leads, atención al cliente automatizada y navegación guiada basada en reglas de negocio.

<img width="1366" height="768" alt="Screenshot_10-Jun_15-52-57_32076" src="https://github.com/user-attachments/assets/c3fc229c-3a83-4880-a1ba-1df3a792b52e" />

<img width="1366" height="768" alt="Screenshot_10-Jun_15-56-15_32483" src="https://github.com/user-attachments/assets/69105ed0-9b9a-4542-9635-08844eb356c4" />



---
*Nota: Este repositorio se mantiene como una exhibición de portafolio para demostrar la implementación de buenas prácticas en el desarrollo de software seguro y soluciones de IA integradas. El código fuente de la lógica interna permanece privado.*
