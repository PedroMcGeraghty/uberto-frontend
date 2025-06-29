# 🚗 Uberto – Frontend Mobile

Uberto es una aplicación de transporte **tipo ride‑sharing** que conecta usuarios y choferes.  
Este repositorio contiene la **interfaz mobile** (SPA) que consume un backend Kotlin + Spring Boot.

## ✨ Características principales
| Rol Usuario | Rol Chofer |
|-------------|------------|
| 🔐 Login único por rol | 🔐 Login único por rol |
| 🔍 Buscar choferes disponibles filtrando origen, destino, fecha y pasajeros | 📑 Listar viajes pendientes |
| 🚕 Reservar viajes y ver resumen antes de confirmar | 💼 Ver historial de viajes y total recaudado |
| 💳 Cargar saldo en la cuenta | ⭐ Ver calificaciones recibidas |
| ⭐ Calificar choferes tras cada viaje | |
| 👤 Gestionar datos de perfil | |

### 🏎️ Tipos de chofer

- **Simple**: plus de $1.000 por minuto.
- **Premium (Ejecutivo)**:
  - $2.000 por minuto si hay 1 pasajero.
  - $1.500 por minuto si hay 2 o más pasajeros.
  - El auto no puede tener más de 10 años de antigüedad.
- **Moto**:
  - $500 por minuto si el viaje dura hasta 30 minutos.
  - $600 por minuto si dura más de 30 minutos.

La comisión de la plataforma es del **5 %** del precio total (base + plus).

---

## 🖼️ Screenshots

### App desde el lado del Pasajero

| Login | 
|-------|
| ![Login](docs/img/login.jpeg) |

| Home (form vacío) | Home (con resultados)   | Confirmación de viaje |
|-----------------------|-----------------------|-----------------------|
| ![Home – empty](docs/img/home-passenger.jpeg) |![Home – results](docs/img/home-search-driver.jpeg) | ![Confirm travel](docs/img/confirm-trip.jpeg)  |

| Perfil del pasajero (Datos Personales) | Dinero disponible del Usuario | Amigos del usuario | 
|-----------------------|-----------------------|-----------------------|
| ![Profile – data](docs/img/profile-data.jpeg) | ![Profile - Balance](docs/img/profile-balance.jpeg) | ![Profile - Friends](docs/img/profile-search-friends.jpeg)

| Viajes pendientes del Pasajero | Viajes completados del pasajero | Calificacion de un viaje | 
|-----------------------|-----------------------|-----------------------|
| ![Profile – Trips Pending](docs/img/profile-pending-trips.jpeg) | ![Profile - Trips Complete](docs/img/profile-complete-trips.jpeg) | ![Profile - Rating finished trip](docs/img/profile-trips-rating.jpeg)

| Calificaciones hechas por el Pasajero |  
|-----------------------|
| ![Profile – Trips Pending](docs/img/profile-ratings.jpeg) | 

### App desde el lado del Chofer

| Login | 
|-------|
| ![Login](docs/img/login-driver.jpeg) |

| Home del chofer (form vacío) | Formulario del chofer (con resultados de viajes pendientes)   
|-----------------------|-----------------------|
| ![Home – empty](docs/img/home-driver.jpeg) |![Home – results](docs/img/home-driver-form.jpeg) 


| Perfil del chofer (Datos Personales) | Fiajes finalizados del chofer | Calificaciones hacia el chofer | 
|-----------------------|-----------------------|-----------------------|
| ![Profile – data](docs/img/profile-driver-data.jpeg) | ![Profile - Trips](docs/img/profile-driver-trips-completed.jpeg) | ![Profile - Ratings](docs/img/profile-driver-ratings.jpeg)


---

## ⚙️ Stack técnico
| Capa | Tecnología |
|------|------------|
| **UI** | React + Vite (TypeScript) + Material UI |
| **Estilos** | CSS |
| **Componentes visuales** | [Material UI (MUI)](https://mui.com/) |
| **Gestor de estado** | Context API / useState / useEffect |
| **Formularios** | [React Hook Form](https://react-hook-form.com/) |
| **Ruteo** | React Router |
| **HTTP client** | Axios |
| **Backend** | Kotlin + Spring Boot (API REST) |

---

## 🚀 Instalación rápida

```bash
# 1. Clonar el repo
git clone https://github.com/<tu-usuario>/uberto-frontend.git
cd uberto-frontend

# 2. Instalar dependencias
npm install        # o pnpm install / yarn

# 3. Correr la aplicación
npm start
