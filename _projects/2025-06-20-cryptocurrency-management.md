---
layout: projects
title: "Sistema de Gestión de Criptomonedas"
date: 2021-06-15
client: ""
duration: "3 meses"
status: "Completado"
category: "Desarrollo Web"
technologies: ["Laravel", "Livewire", "Javascript", "Bootstrap"]
tags: ["desarrollo web", "laravel", "bitcoin", "tether"]
image: "/assets/images/projects/cryptocurrency/banner_cryptocurrency_project.png"
gallery:
  - "/assets/images/projects/cryptocurrency/cryptocurrency_users_approved.png"
  - "/assets/images/projects/cryptocurrency/cryptocurrency_comissions.png"
  - "/assets/images/projects/cryptocurrency/cryptocurrency_limit_purchase.png"
---

## 📈 Resumen del Proyecto

Este proyecto involucró el desarrollo de un **sistema integral de gestión de criptomonedas** que permite administrar clientes, personal empresarial y operaciones de compra de Bitcoin (BTC) y Tether (USDT) a través de plataformas externas, manteniendo un control administrativo completo y registro detallado de todas las transacciones.

### 🚀 Características Principales Implementadas

#### **Gestión de Clientes**

- 👥 Sistema de aprobación/rechazo de clientes
- 🔒 Funcionalidad de bloqueo y desbloqueo de usuarios
- 📋 Panel de administración de estados de cuenta
- ✅ Proceso de verificación y validación de usuarios
- 📊 Historial completo de actividades por cliente

#### **Administración de Personal**

- 🏢 Gestión completa de empleados de la empresa
- 💰 Sistema de control de salarios y nómina
- 👤 Perfiles de empleados con roles y permisos
- 🎯 Asignación de responsabilidades y departamentos

#### **Control de Operaciones**

- 💳 Configuración de límites de compra por usuario
- 💼 Sistema de comisiones por envío personalizable
- 🔗 Integración con plataformas externas de trading
- 📈 Registro y seguimiento de transacciones Bitcoin/Tether

## 🏗️ Arquitectura Técnica

### 🖥️ Stack Tecnológico Principal

La plataforma utiliza una **arquitectura MVC robusta** construida con tecnologías modernas de PHP:

| Componente | Tecnología | Función |
|------------|------------|---------|
| 🔧 **Backend Framework** | Laravel | Core del sistema y lógica de negocio |
| ⚡ **Frontend Dinámico** | Livewire | Componentes reactivos sin JavaScript complejo |
| 🎨 **UI Framework** | Bootstrap | Diseño responsivo y componentes UI |
| 🔄 **Interactividad** | JavaScript | Funcionalidades del lado del cliente |
| 🗄️ **Base de Datos** | MySQL  | Almacenamiento de datos principal |

## 💪 Desafíos Superados

### 🔐 **Gestión de Estados de Usuario**
>
> **Problema**: Necesidad de un sistema robusto para **aprobar, rechazar y bloquear** usuarios de manera eficiente.
>
> **Solución**: Implementamos un sistema de estados permite cambios y notificaciones automáticas para la gestión de los usuarios

### 🏢 **Administración de Personal Compleja**
>
> **Problema**: Gestionar múltiples aspectos del personal (liquidaciones, roles, cargos).
>
> **Solución**: Desarrollamos módulos especializados con `Laravel Eloquent` para relaciones complejas y generación de liquidaciones.

## 🔮 Características del Sistema

### 👥 **Módulo de Gestión de Clientes**

| Funcionalidad | Descripción |
|---------------|-------------|
| ✅ **Aprobación** | Sistema de revisión y aprobación de nuevos clientes |
| ❌ **Rechazo** | Proceso documentado para rechazar solicitudes |
| 🔒 **Bloqueo/Desbloqueo** | Control granular de acceso de usuarios |
| 📊 **Dashboard** | Panel con métricas y estado de cada cliente |

### 🏢 **Módulo de Recursos Humanos**

| Funcionalidad | Descripción |
|---------------|-------------|
| 👤 **Gestión de Empleados** | Registro, edición y eliminación de perfiles de empleados |
| 💰 **Control de liquidaciones** | Gestión e historial de liquidaciones |
| 🏛️ **Cargos** | Asignación de cargos de los empleados |
| 📅 **Asistencia** | Seguimiento de horarios y control de ausencias |
| 📊 **Reportes de RH** | Estadísticas y métricas del personal |

### 💳 **Sistema de Límites y Comisiones**

| Funcionalidad | Descripción |
|---------------|-------------|
| 💵 **Límites de Compra** | Configuración de montos máximos por usuario |
| 📈 **Comisiones Variables** | Cálculo automático de comisiones por tipo de transacción |
| 📊 **Monitoreo de Límites** | Alertas automáticas por proximidad a límites |
| 💼 **Comisiones por Envío** | Tarifas personalizables según método y destino |
