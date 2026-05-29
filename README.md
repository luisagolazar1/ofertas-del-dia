# 🏷️ Ofertas del Día

App personal para registrar y consultar ofertas, reintegros y descuentos de bancos y billeteras en Argentina. Funciona 100% en el navegador, sin servidor, y se puede hostear gratis en GitHub Pages.

## ✨ Funcionalidades

- 📅 **Filtro por día de semana** — muestra automáticamente las ofertas del día actual
- 📂 **Categorías** — Supermercados, Combustible, Gastronomía, Farmacia, Indumentaria, Electrónica, Entretenimiento, Viajes
- 🔄 **Auto-actualización** — busca promos vigentes en la web usando Claude AI con búsqueda web
- 📥 **Preview de importación** — revisás y elegís qué ofertas importar antes de guardar
- 🤖 **Consulta de veracidad** — le preguntás a Claude sobre las ofertas cargadas
- 💾 **Persistencia local** — los datos se guardan en `localStorage` del navegador
- 📱 **Mobile-first** — diseñado para funcionar bien en celular

## 🚀 Uso en GitHub Pages

### 1. Subir el repositorio

```bash
git clone https://github.com/TU_USUARIO/ofertas-del-dia.git
cd ofertas-del-dia
# Copiá el index.html aquí
git add .
git commit -m "Initial commit"
git push
```

### 2. Activar GitHub Pages

En tu repositorio: **Settings → Pages → Source: Deploy from branch → main / root**

Tu app estará en: `https://TU_USUARIO.github.io/ofertas-del-dia`

### 3. Configurar API Key

Para usar la **auto-actualización** y el **chat con Claude** fuera de Claude.ai necesitás una API Key de Anthropic:

1. Entrá a [console.anthropic.com](https://console.anthropic.com) y creá una API Key
2. En la app, tocá **⚙️ Configuración**
3. Pegá tu API Key y guardá

> **La key se guarda solo en tu dispositivo** (`localStorage`). Nunca se envía a ningún servidor propio.

## 💡 Uso de la auto-actualización

1. En ⚙️ Configuración, activá los proveedores que querés buscar
2. Tocá **🔄 Actualizar ofertas**
3. Claude busca en la web las promos vigentes
4. Revisás las ofertas encontradas y elegís cuáles importar

> ⚠️ Los resultados dependen de lo que Claude encuentre en la web. Verificá siempre en el sitio oficial de cada banco/billetera antes de usarlos.

## 📁 Estructura

```
ofertas-del-dia/
└── index.html   # App completa, un solo archivo
└── README.md
```

## 🛠️ Tecnologías

- HTML/CSS/JS vanilla — sin frameworks, sin build step
- [Anthropic API](https://docs.anthropic.com) con `web_search` tool
- Google Fonts (Syne + DM Sans)
- localStorage para persistencia

## ⚠️ Disclaimer

Los datos de las ofertas son ingresados manualmente o sugeridos por IA. No son datos oficiales. Verificá siempre las condiciones en el sitio del banco o billetera correspondiente.
