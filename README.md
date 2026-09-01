# jennifer

Invitación web para los XV años de **Jennifer Casillas**.

- **Fecha:** viernes 02 de octubre de 2026, 8:00 p.m.
- **Lugar:** Terraza Jardín Duranta — Sta. María 875, La Micailita, 45595 San Pedro Tlaquepaque, Jal.
- **Contacto:** 33 2199 3378

## Archivos

| Archivo | Descripción |
|---|---|
| `index.html` | La invitación completa |
| `generar.html` | Generador de enlaces personalizados por invitado |

## Enlaces personalizados

`generar.html` arma la liga de cada invitado con estos parámetros:

| Parámetro | Significado | Ejemplo |
|---|---|---|
| `f` | Nombre de la familia o invitado | `?f=Familia%20García` |
| `t` | Tipo de saludo: `familia`, `estimado`, `estimada` | `&t=familia` |
| `b` | Número de boletos | `&b=4` |
| `m` | Mesa (opcional) | `&m=5` |

Ejemplo: `index.html?f=Familia%20García&t=familia&b=4&m=5`

## Confirmaciones

El formulario de la invitación envía por POST los campos `nombre`, `asistencia` y `mensaje`
a un Google Apps Script, que los escribe en la hoja de confirmaciones.
