# Tokeniza-IA

Cotizador de proyectos de IA: 10 preguntas de opción múltiple que recomiendan el tipo de agente y el modelo, con costo por conversación y mensual, sensibilidad y palancas de ahorro.

- Un solo archivo (`index.html`), funciona sin internet.
- Cuenta tokens exactos con el tokenizer de OpenAI (o200k_base, js-tiktoken 1.0.21) incluido en el archivo.
- Fórmula por conversación: Entrada = T·S + (u+a)·T(T−1)/2 + T·u + O; Salida = T·(a + razonamiento); Costo = (Entrada × Pin + Salida × Pout) / 1,000,000.

**Limitaciones**
- Tarifas de [GPT for Work](https://gptforwork.com/tools/openai-chatgpt-api-pricing-calculator) al 2026-10-09 (agregador; contrastar con la página oficial de cada proveedor). Editables en Ajustes.
- Conteo exacto solo para modelos de OpenAI; aproximado para Claude, Gemini y otros.
- El nivel de capacidad de cada modelo es una clasificación de referencia, no un benchmark.
- Solo costo de API: no incluye suscripciones, canal (WhatsApp/SMS), infraestructura ni personas.
