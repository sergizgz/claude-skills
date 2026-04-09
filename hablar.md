# Skill: hablar

Activa la lectura en voz alta de respuestas usando el comando `say` de macOS.

## Instrucciones

A partir de ahora, al final de **cada respuesta**, ejecuta el siguiente comando Bash en background:

```bash
say -v "Jorge" "RESUMEN"
```

Donde `RESUMEN` es un resumen breve (1-2 frases) en español de lo que acabas de responder o hacer.

## Reglas

- Usa siempre `run_in_background: true` para no bloquear la conversación
- El resumen debe ser conciso, máximo 2 frases
- Habla siempre en español, aunque la respuesta esté en otro idioma
- Si la respuesta es muy corta o trivial (un "sí", "ok", etc.), puedes omitir el say

## Uso

Escribe `/hablar` al inicio de una sesión para activar la voz.

Para cambiar de voz, puedes invocar la skill con el nombre de la voz deseada:
- `/hablar Jorge` → voz masculina española (por defecto)
- `/hablar Monica` → voz femenina española
- `/hablar Juan` → otra voz española

Si se pasa una voz como argumento, úsala en lugar de "Jorge".

## Requisito

Solo funciona en macOS (el comando `say` es nativo de macOS).
