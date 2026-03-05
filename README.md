# 🎙️ AgentFlow — Guía de despliegue en Vercel

## Estructura del proyecto
```
agentflow/
├── api/
│   └── generate.js      ← Función serverless (llama a Claude de forma segura)
├── public/
│   └── index.html       ← La plataforma completa
├── vercel.json          ← Configuración de Vercel
├── package.json
└── README.md
```

---

## 🚀 PASOS PARA PUBLICAR

### 1. Sube esto a GitHub
- Ve a github.com → "New repository" → nombre: `agentflow`
- Sube todos estos archivos (arrastra la carpeta o usa git)

### 2. Conecta con Vercel
- Ve a vercel.com → "Add New Project"
- Elige tu repo `agentflow` de GitHub
- Click en "Deploy" (sin tocar nada más)

### 3. Añade tu API Key de Anthropic
- En Vercel → tu proyecto → "Settings" → "Environment Variables"
- Añade:
  - Name: `ANTHROPIC_API_KEY`
  - Value: `sk-ant-api03-...` (tu clave de console.anthropic.com)
- Click "Save" → luego "Redeploy"

### 4. ¡Listo!
Tu URL será: `https://agentflow-xxxx.vercel.app`

---

## 🔑 Cómo obtener la API Key de Anthropic (GRATIS)
1. Ve a https://console.anthropic.com
2. Crea cuenta con tu email
3. Ve a "API Keys" → "Create Key"
4. Copia la clave que empieza por `sk-ant-...`
5. Tienes $5 de crédito gratis al registrarte

---

## 💡 Funcionalidades incluidas
- ✅ Crear agentes con un solo prompt en lenguaje natural
- ✅ Claude genera automáticamente: nombre, rol, system prompt, voz, escenarios
- ✅ Biblioteca de voces ElevenLabs (preview)
- ✅ Escenarios Make.com (citas, leads, recordatorios)
- ✅ Dashboard con métricas
- ✅ Configuración de API keys

---

## 🔧 Próximas integraciones a añadir
- [ ] ElevenLabs API (audio real de voces)
- [ ] Twilio (llamadas telefónicas reales)
- [ ] Make.com webhooks (automatizaciones reales)
- [ ] Supabase (base de datos para guardar agentes)
