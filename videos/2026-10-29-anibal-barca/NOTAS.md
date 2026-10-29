# Estado: INCOMPLETO (bloqueado por servicios externos)

Fecha: 2026-10-29. Tema: Aníbal Barca.

## Hecho
- `script.txt` recortado a 326 palabras.
- 3 imágenes generadas en Higgsfield (retrato, juramento, Cannas) pero NO se pudieron descargar: ver bloqueo 3.

## Bloqueos
1. **Higgsfield sin créditos**: plan free, balance = 0. De 10 imágenes pedidas en batch, solo 3 se aceptaron;
   las otras 7 (Alpes, elefante, Roma desde la colina, Zama, exilio, soldados, pánico en el foro) fallaron con
   "Out of credits on free plan". Prompts pendientes: ver historial del intento (escenas 2,3,5,6,7,8,9).
2. **TTS**: `npx hyperframes tts` falla: falta `kokoro-onnx` (`pip install kokoro-onnx soundfile`). No se instaló
   ni se continuó por la instrucción de no insistir tras un bloqueo externo.

3. **Descarga bloqueada**: el firewall devuelve 403 en CONNECT a d8j0ntlcm91z4.cloudfront.net (CDN de Higgsfield),
   así que las imágenes generadas no se pueden bajar al repo. URLs de resultado (job ids):
   - 1a31fb57-4325-4ece-8401-daafb1b7bfc0 (retrato)
   - 8af0cfbe-5e26-4376-94f8-5b997b6fd320 (juramento)
   - 12f26f1f-5d9a-4913-a247-963ab7fac50d (Cannas)

## Pendiente
Recargar créditos de Higgsfield, generar las 7 imágenes restantes, instalar kokoro-onnx, correr tts + transcribe,
armar el proyecto HyperFrames, renderizar y recién ahí agregar "Aníbal Barca" a `videos/topics_used.json`
(NO agregado todavía).
