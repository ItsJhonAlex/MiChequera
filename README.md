# MyPecuny

Aplicación móvil para la gestión de finanzas personales con categorización avanzada y asistencia mediante IA.

---

## 🚀 Descripción

MyPecuny te ayuda a llevar el control de tus finanzas personales, categorizando ingresos y gastos, y ofreciéndote recomendaciones inteligentes gracias a la integración con IA (Google Gemini).

---

## 🛠️ Stack Tecnológico

- **Frontend:** Flutter (cross-platform)
- **Backend:** Supabase (PostgreSQL, Auth, Storage, Edge Functions)
- **IA:** Google Gemini (API key configurable por el usuario)

---

## 🏗️ Arquitectura: Clean Architecture

El proyecto sigue el patrón de Clean Architecture, separando responsabilidades en capas para facilitar la escalabilidad, pruebas y mantenibilidad.

```
/lib
  /core            # Utilidades y helpers generales
  /features
    /auth          # Autenticación y perfil
    /finance       # Finanzas: cuentas, transacciones, categorías
    /analysis      # Análisis y reportes
    /ai            # Integración con Gemini
  /models          # Modelos de dominio
  /services        # Servicios externos (Supabase, IA)
  /providers       # Gestión de estado (Provider/BLoC)
  /widgets         # Widgets reutilizables
  /l10n            # Internacionalización
  /theme           # Temas y estilos
  /utils           # Utilidades varias
/assets            # Recursos estáticos
/test              # Pruebas
```

**Ventajas:**
- Separación clara de lógica de negocio, presentación y datos.
- Fácil de testear y escalar.
- Permite reemplazar tecnologías (ej: cambiar Supabase) sin afectar el resto del sistema.

---

## ⚡ Instalación Rápida

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu_usuario/mypecuny.git
   cd mypecuny
   ```

2. Instala dependencias:
   ```bash
   flutter pub get
   ```

3. Configura Supabase para Android/iOS siguiendo la [guía oficial](https://supabase.com/docs/guides/getting-started).

4. Ejecuta la app:
   ```bash
   flutter run
   ```

---

## 🧩 Comandos Útiles

- Ejecutar en modo debug:
  ```bash
  flutter run
  ```
- Ejecutar pruebas:
  ```bash
  flutter test
  ```

---

## 💡 Buenas Prácticas

- Commits siguiendo [Conventional Commits](https://www.conventionalcommits.org/es/v1.0.0/).
- Variables sensibles fuera del repositorio.
- Código documentado y modular.
- Pruebas unitarias y de integración.

---

## 📄 Licencia

MIT

---

## 👩‍💻 Créditos

Desarrollado por el equipo MyPecuny.
