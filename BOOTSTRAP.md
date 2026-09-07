# BOOTSTRAP — AUDITOR

## Constitución

```text
WORK_ID=prueba-orquestador-e2e-relevos-manuales-ai
CARRIL=L
ROL=AUDITOR
```

Este archivo preserva los hechos de constitución recibidos en el arranque externo. No declara estado vivo del trabajo.

## Manifiesto aprobado

```text
MANIFEST_REPO=https://github.com/francogg89-ai/manifiestos-trabajo-ai
MANIFEST_PATH=manifiestos/prueba-orquestador-e2e-relevos-manuales-ai/MANIFIESTO_TRABAJO.md
MANIFEST_SHA=8ec61409a71550d0595a137abd2ce7f470560055
PROJECT.md=NO_EXISTE
```

## Método gobernante

```text
METHOD_REPO=https://github.com/francogg89-ai/orchestra-revolutions-ai
METHOD_SHA=4d88fce3ed3c87bd231c45ec60dcb713538b2514
METHOD_PATHS=
- metodo/REVOLUTIONS.md
- metodo/ROL-AUDITOR.md
- metodo/ROL-CONSTRUCTOR.md
```

## Fuentes constitutivas y de transporte

```text
RULES_REPO=https://github.com/francogg89-ai/rules-orchestrator-ai
RULES_PATH=REGLAS-ORQUESTADOR.md
RULES_SHA=d2e6be55c74b7aea26694c2007ea3bb74f21642e

MANIFEST_METHOD_REPO=https://github.com/francogg89-ai/metodo-manifiestos-ai
MANIFEST_METHOD_SHA=9f2c3f0de92f5f6988bdbd2753140fa5cc93a0d8
```

Esas fuentes son de sólo lectura durante esta corrida.

## Repositorios de ejecución

```text
WORK_REPO=https://github.com/francogg89-ai/work-claude-l
AUDIT_REPO=https://github.com/francogg89-ai/audit-chatgpt-l
```

Fronteras estructurales:

- CONSTRUCTOR escribe exclusivamente en `work-claude-l` y no escribe en `audit-chatgpt-l`.
- AUDITOR escribe exclusivamente en `audit-chatgpt-l` y no escribe en `work-claude-l`.
- ORQUESTADOR transporta y no escribe por cuenta de los actores.

## Entorno local

```text
ROOT_LOCAL=C:\Franco_Metodos_AI

LOCAL_PATHS:
RULES_ORCHESTRATOR=C:\Franco_Metodos_AI\rules-orchestrator-ai
WORK=C:\Franco_Metodos_AI\work-claude-l
AUDIT=C:\Franco_Metodos_AI\audit-chatgpt-l
METODO_MANIFIESTOS=C:\Franco_Metodos_AI\metodo-manifiestos-ai
MANIFIESTOS=C:\Franco_Metodos_AI\manifiestos-trabajo-ai
METHOD=C:\Franco_Metodos_AI\orchestra-revolutions-ai
```

Los repositorios relevantes están disponibles localmente bajo `C:\Franco_Metodos_AI`.

## Runtimes

```text
AUDITOR=conversación de ChatGPT
CONSTRUCTOR=Claude Code local en Windows
CONSTRUCTOR_LOCAL_PATH=C:\Franco_Metodos_AI\work-claude-l
```

## Capacidades inicialmente delegadas

### CONSTRUCTOR

```text
ACTOR=CONSTRUCTOR
ENTORNO=clones locales bajo C:\Franco_Metodos_AI
CAPACIDAD=lectura de las fuentes constitutivas y metodológicas necesarias
LIMITES=solo lectura fuera de work-claude-l

ACTOR=CONSTRUCTOR
ENTORNO=C:\Franco_Metodos_AI\work-claude-l
CAPACIDAD=construcción y escritura material
LIMITES=exclusivamente work-claude-l; no escribir en audit-chatgpt-l
```

### AUDITOR

```text
ACTOR=AUDITOR
ENTORNO=repositorios Git constitutivos y de ejecución accesibles
CAPACIDAD=lectura e inspección independiente de las identidades exactas necesarias
LIMITES=sin modificación del candidato material

ACTOR=AUDITOR
ENTORNO=https://github.com/francogg89-ai/audit-chatgpt-l
CAPACIDAD=escritura durable de constitución y auditoría
LIMITES=exclusivamente audit-chatgpt-l; no escribir en work-claude-l
```

No se recibieron valores de secretos ni referencias a credenciales necesarias para esta prueba.

## Políticas iniciales materialmente declaradas

La autoridad material es el manifiesto exacto citado arriba. En particular, la constitución declara una prueba de cinco entregas principales del CONSTRUCTOR posteriores al establecimiento y aprobación del PLAN, cada una auditada antes de continuar.

No existen relevos periódicos automáticos de CONSTRUCTOR ni de AUDITOR. Los relevos se ejercitan únicamente por directiva del HUMANO durante una pausa y son procesados metodológicamente por el actor competente conforme a REVOLUTIONS.

La corrida debe atravesar al menos una secuencia `DETENER` / directiva humana / continuación, al menos un relevo manual efectivo con una instancia `fresh` real y continuidad posterior por `current`, reconstrucción desde Git por una instancia fresca y aprobación humana del PLAN cuando corresponda.

No se mantienen contadores vivos ni estado metodológico paralelo.

## Próxima acción constitutiva

```text
PROXIMA_ACCION=Constituir al primer CONSTRUCTOR como instancia fresh en C:\Franco_Metodos_AI\work-claude-l, entregándole la constitución necesaria, la identidad exacta de este BOOTSTRAP y la instrucción de crear su propio BOOTSTRAP, sincronizar fuentes y producir el PLAN mínimo compatible con el manifiesto.
PERIMETRO_ULTIMA_MODIFICACION=CONSTITUCION
```
