# Wang Plus Ticket 🎫

**Sistema de Gestión de Tickets y Workflows Visuales con Next.js y React Flow**

Un proyecto moderno para la gestión integral de tickets con visualización interactiva de flujos de trabajo usando React Flow.

## 🌟 Características Principales

### 📊 Visualización de Workflows
- Interfaz visual e interactiva basada en **React Flow**
- Diagramas de flujo personalizables para procesos de tickets
- Conexiones dinámicas entre estados y acciones
- Soporte para nodos personalizados

### 🎫 Gestión de Tickets
- Sistema CRUD completo para tickets
- Estados configurables (Abierto, En Progreso, Cerrado, etc.)
- Asignación de responsables
- Prioridades y categorías
- Historial de cambios

### 🔐 Autenticación y Seguridad
- NextAuth.js para autenticación segura
- Control de roles y permisos
- Protección de rutas

### 📈 Análisis y Reportes
- Dashboards con estadísticas en tiempo real
- Gráficos con Recharts
- Exportación de reportes

### 🎨 UI Moderna
- Interfaz construida con Tailwind CSS
- Componentes accesibles con Radix UI
- Iconos con Lucide React
- Notificaciones con React Hot Toast

## 🛠️ Stack Tecnológico

| Tecnología | Versión | Propósito |
|-----------|---------|----------|
| **Next.js** | ^14.0.0 | Framework React fullstack |
| **React** | ^18.2.0 | Librería UI |
| **React Flow** | ^11.10.0 | Visualización de workflows |
| **TypeScript** | ^5.3.2 | Tipado estático |
| **Tailwind CSS** | ^3.3.6 | Estilos utilitarios |
| **React Hook Form** | ^7.48.0 | Gestión de formularios |
| **NextAuth.js** | ^4.24.9 | Autenticación |
| **Axios** | ^1.6.2 | Cliente HTTP |
| **Zustand** | ^4.4.1 | State management |
| **Recharts** | ^2.10.3 | Gráficos |

## 📁 Estructura del Proyecto

```
wang_plus_ticket/
├── src/
│   ├── app/                    # App router de Next.js
│   ├── components/             # Componentes reutilizables
│   │   ├── workflow/          # Componentes de React Flow
│   │   ├── tickets/           # Componentes de gestión de tickets
│   │   └── common/            # Componentes comunes
│   ├── pages/                 # Páginas de la aplicación
│   ├── lib/                   # Utilidades y configuraciones
│   ├── hooks/                 # Custom hooks
│   ├── types/                 # Definiciones TypeScript
│   ├── styles/                # Estilos globales
│   └── api/                   # Rutas API
├── public/                    # Assets estáticos
├── package.json
├── tsconfig.json
├── next.config.js
├── tailwind.config.js
└── README.md
```

## 🚀 Instalación y Uso

### Requisitos Previos
- Node.js 18.x o superior
- npm, yarn, pnpm o bun

### Pasos de Instalación

1. **Clonar el repositorio**
```bash
git clone https://github.com/DidierDev672/wang_plus_ticket.git
cd wang_plus_ticket
```

2. **Instalar dependencias**
```bash
npm install
# o
yarn install
# o
pnpm install
```

3. **Configurar variables de entorno**
```bash
cp .env.example .env.local
```

4. **Ejecutar en desarrollo**
```bash
npm run dev
```

5. **Acceder a la aplicación**
```
http://localhost:3000
```

## 📝 Scripts Disponibles

```bash
npm run dev          # Iniciar servidor de desarrollo
npm run build        # Compilar para producción
npm start            # Iniciar servidor de producción
npm run lint         # Ejecutar ESLint
npm run type-check   # Verificar tipos TypeScript
```

## 🎨 Componentes Principales

### WorkflowEditor
Editor visual de workflows usando React Flow
```typescript
<WorkflowEditor 
  nodes={nodes}
  edges={edges}
  onNodesChange={handleNodesChange}
  onEdgesChange={handleEdgesChange}
/>
```

### TicketManager
Gestor completo de tickets
```typescript
<TicketManager 
  tickets={tickets}
  onCreateTicket={handleCreate}
  onUpdateTicket={handleUpdate}
/>
```

### DashboardStats
Estadísticas y análisis
```typescript
<DashboardStats 
  totalTickets={100}
  openTickets={25}
  closedTickets={75}
/>
```

## 🔄 Flujo de Trabajo Típico

1. **Crear Workflow** - Diseña el flujo de procesos visualmente
2. **Crear Ticket** - Inicia un nuevo ticket en el workflow
3. **Asignar Responsable** - Asigna el ticket a un usuario
4. **Seguimiento** - Monitorea el progreso en el dashboard
5. **Cierre** - Completa y archiva el ticket

## 🔐 Variables de Entorno

```env
# API
NEXT_PUBLIC_API_URL=http://localhost:3000/api

# Autenticación
NEXTAUTH_SECRET=tu_secreto_aqui
NEXTAUTH_URL=http://localhost:3000

# Base de Datos
DATABASE_URL=tu_url_base_datos

# Email (Opcional)
EMAIL_SERVER_HOST=smtp.gmail.com
EMAIL_SERVER_PORT=587
EMAIL_SERVER_USER=tu_email@gmail.com
EMAIL_SERVER_PASSWORD=tu_contraseña
EMAIL_FROM=noreply@wangplus.com
```

## 🎯 Casos de Uso

- **Helpdesk** - Sistema de soporte técnico
- **Gestión de Proyectos** - Seguimiento de tareas
- **Flujos de Aprobación** - Procesos de validación
- **Soporte al Cliente** - Gestión de incidencias
- **Recursos Humanos** - Procesos de solicitud

## 📚 Documentación Adicional

- [React Flow Documentation](https://reactflow.dev)
- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com)
- [React Hook Form](https://react-hook-form.com)

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit de cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo LICENSE para detalles.

## 👨‍💻 Autor

**Didier Arias** - [GitHub](https://github.com/DidierDev672)

## 📞 Soporte

Para soporte, abre un issue en el repositorio o contacta a través de:
- Email: didier@wangplus.com
- GitHub Issues: [Wang Plus Ticket Issues](https://github.com/DidierDev672/wang_plus_ticket/issues)

---

⭐ Si este proyecto te fue útil, por favor considera darle una estrella en GitHub
