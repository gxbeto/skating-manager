# skating-manager

Sistema de gestión para academia de patinaje:

- Registro de atletas y responsables
- Gestión de documentación (PDF/Imágenes)
- Gestión deportiva (modalidades, niveles y categorías)
- Cobranza / cuenta corriente (cuotas, cobros por evento, pagos parciales, extractos)
- Gestión básica de personal
- (Opcional) Libro simple de ingresos y egresos

---

## Tecnologías

- **Frontend:** Flutter
- **Backend:** Python (API)
- **Base de datos:** _por definir_
- **Almacenamiento de adjuntos:** _por definir_

---

## Estructura del repositorio (sugerida)

/mobile/ -> App Flutter

/backend/ -> API en Python (reglas de negocio + endpoints)

/shared/ -> Contratos compartidos (DTOs/Schemas)

/docs/ -> Documentación funcional y técnica

/scripts/ -> Scripts de soporte (setup, seed, etc.)
---

## Requisitos previos

- Flutter SDK instalado
- Python **3.11+** (recomendado)
- Git

---

## Cómo ejecutar (básico)

### 1) Clonar

`bash

git clone <URL_DEL_REPO>
cd skating-manager


*2) Backend (Python)*
cd backend
python -m venv .venv
# Windows
.venv\Scripts\activate
# Linux/Mac
# source .venv/bin/activate

pip install -r requirements.txt
python main.py

*3) App (Flutter)*
cd ../mobile
flutter pub get
flutter run

---

Configuración

Crear un archivo .env (o el que defina el backend) con variables como:

DATABASE_URL=
STORAGE_PATH= (o S3 compatible)
SECRET_KEY=
ALLOWED_ORIGINS=



