# Registro de Decisiones Técnicas (DECISIONS.md) - Semana 2

## Decisión 1: Remoción Absoluta de Contraseña y Autenticación Tradicional
* **Contexto:** En las pruebas con usuarios informales de Capa 1 (Doña Mari), exigir un correo electrónico y una contraseña provocaba un abandono inmediato del 100% de los usuarios debido al olvido de credenciales y desconfianza.
* **Solución Aplicada:** Se eliminó el flujo tradicional de login y la dependencia de Google Providers en Supabase. Se implementó un "Acceso Seguro en Un Clic" (Modo Demo) para garantizar la inclusión y permitir la navegación inmediata hacia el formulario narrativo.

## Decisión 2: Simulación Local de Estructuración de Datos de IA
* **Contexto:** Para mitigar el bloqueo por cuotas o falta de créditos en APIs externas de generación en vivo durante el desarrollo local, se requería una alternativa robusta para la entrega visual.
* **Solución Aplicada:** El procesamiento del modelo de lenguaje se simula mediante una función nativa en JavaScript que recibe el lenguaje informal del usuario y devuelve en pantalla una estructura JSON limpia ("Tarjeta de Confianza Técnica"), aislando por completo variables de exclusión como el historial en buró o la geolocalización discriminatoria.
