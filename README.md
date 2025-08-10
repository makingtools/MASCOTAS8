# Pet-Tech Connect

**Pet-Tech Connect** es una plataforma web de vanguardia que demuestra la fusión de servicios de cuidado de mascotas con funcionalidades avanzadas de inteligencia artificial. El proyecto está diseñado para ser un escaparate de una experiencia de usuario interactiva y moderna, tanto para los dueños de mascotas (B2C) como para los socios comerciales (B2B).

![Pet-Tech Connect Landing Page](https://images.unsplash.com/photo-1537151625747-768eb6cf92b2?auto=format&fit=crop&w=1280&q=80)

---

## ✨ Características Principales

### Para Clientes (B2C)
- **Página de Aterrizaje Interactiva:** Un diseño moderno y atractivo con microanimaciones, efectos de scroll y un diseño completamente responsivo.
- **Servicios de Autolavado:** Tres niveles de servicio de autolavado para perros, detallados y con precios.
- **Asistente de IA "Conecty":** Un chatbot multimodal que puede:
  - Agendar citas utilizando un flujo de conversación natural.
  - Navegar por la página web.
  - Abrir otras herramientas de IA.
  - Reconocimiento y síntesis de voz en múltiples idiomas.
- **Escáner de Razas con IA:** Sube una foto de un perro y la IA identificará su raza o mezcla de razas.
- **Generador de Arte con IA:** Transforma una foto de tu mascota en una obra de arte en diferentes estilos artísticos.

### Para Socios (B2B)
- **Panel de Administrador Seguro:** Acceso mediante contraseña o cuenta de Google.
- **Dashboard Interactivo y Optimizado:** Gracias a la carga perezosa (`React.lazy`), el panel carga increíblemente rápido, mostrando cada sección bajo demanda.
- **Gestión Integral:** Módulos completos para gestionar:
  - **Clientes:** Fichas de clientes con historial de mascotas, citas y comunicación.
  - **Citas:** Visualización y gestión del calendario de citas.
  - **Leads:** Captura y seguimiento de clientes potenciales B2B.
  - **Marketing:** Creación y envío de campañas promocionales.
  - **Finanzas:** Gestión de proveedores, gastos e inventario.
- **Asistente IA para Administradores:** "Conecty" en el panel puede ejecutar acciones administrativas complejas (cancelar citas, confirmar pagos, obtener resúmenes financieros, enviar campañas de marketing) directamente desde el chat.
- **Integración con Google Workspace:** Funcionalidad para sincronizar citas con Google Calendar, crear copias de seguridad en Google Drive y exportar datos a Google Sheets.
- **Configuración del Sistema:** Personalización de marca, servicios y gestión de usuarios del panel.
- **Simulador de Despliegue:** Una función para simular el despliegue de la aplicación a producción.

---

## 🛠️ Pila Tecnológica

- **Frontend:** React 19, TypeScript
- **Estilos:** TailwindCSS
- **Inteligencia Artificial:** Google Gemini API (gemini-2.5-flash para texto, imagen-3.0-generate-002 para imágenes)
- **Gestión de Dependencias:** ES Modules con `importmap` (sin bundler)
- **Internacionalización:** React Context API para soporte de español e inglés.
- **API de Navegador:** Web Speech API (SpeechSynthesis y SpeechRecognition)
- **Servidor de Desarrollo:** `live-server`

---

## 🚀 Instalación y Ejecución

Sigue estos pasos para poner en marcha el proyecto en tu máquina local.

### Prerrequisitos
- [Node.js](https://nodejs.org/) (versión 18 o superior)
- Navegador web moderno (Chrome, Firefox, Edge)

### 1. Clonar el Repositorio
```bash
git clone https://github.com/tu-usuario/pet-tech-connect.git
cd pet-tech-connect
```

### 2. Instalar Dependencias
Este proyecto utiliza `live-server` para el desarrollo. Instálalo como dependencia de desarrollo.
```bash
npm install
```

### 3. Configurar Variables de Entorno
Necesitas una clave de API de Google Gemini para que las funcionalidades de IA funcionen.

1.  Crea un archivo `.env` en la raíz del proyecto, copiando el ejemplo:
    ```bash
    cp .env.example .env
    ```
2.  Obtén tu clave de API gratuita desde [Google AI Studio](https://aistudio.google.com/app/apikey).
3.  Abre el archivo `.env` y pega tu clave:
    ```
    API_KEY="TU_API_KEY_AQUI"
    ```

### 4. Ejecutar la Aplicación
Usa el script de `npm` para iniciar el servidor de desarrollo.
```bash
npm start
```
`live-server` iniciará y abrirá automáticamente la aplicación en tu navegador. ¡Y listo! La aplicación debería estar funcionando localmente.

---

## 🔐 Contraseña de Administrador

Para acceder al panel de administrador sin una cuenta de Google, puedes usar la contraseña definida en el código:
- **Archivo:** `constants.tsx`
- **Contraseña:** `J0j4t4n***`

Esta contraseña es solo para fines de demostración.