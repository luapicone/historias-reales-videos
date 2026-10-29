# Estado: INCOMPLETO (bloqueado por servicios externos)

Fecha: 2026-10-29. Tema: Aníbal Barca.

## Hecho
- `script.txt` recortado a 326 palabras.
- 3 imágenes generadas con Higgsfield (`assets/images/`): retrato, juramento, Cannas.

## Bloqueos
1. **Higgsfield sin créditos**: plan free, balance = 0. De 10 imágenes pedidas en batch, solo 3 se aceptaron;
   las otras 7 (Alpes, elefante, Roma desde la colina, Zama, exilio, soldados, pánico en el foro) fallaron con
   "Out of credits on free plan". Prompts pendientes: ver historial del intento (escenas 2,3,5,6,7,8,9).
2. **TTS**: `npx hyperframes tts` falla: falta `kokoro-onnx` (`pip install kokoro-onnx soundfile`). No se instaló
   ni se continuó por la instrucción de no insistir tras un bloqueo externo.

## Pendiente
Recargar créditos de Higgsfield, generar las 7 imágenes restantes, instalar kokoro-onnx, correr tts + transcribe,
armar el proyecto HyperFrames, renderizar y recién ahí agregar "Aníbal Barca" a `videos/topics_used.json`
(NO agregado todavía).
