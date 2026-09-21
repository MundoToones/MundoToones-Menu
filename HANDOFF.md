# Handoff Summary — 2026-09-21 06:12

## Goal
Menú digital estático para "Comidas Rápidas Mundo Tunes" publicable en GitHub Pages. HTML/CSS puro con personajes Looney Tunes como SVGs.

## Current State

**Lo que está funcionando:**
- 17 cards con personajes SVG (uno por card), sistema `has-char` / `char-bottom`
- Animación flip al scroll con `IntersectionObserver` en cards y títulos
- Vista desktop: personajes salen por arriba (`top` negativo) o por abajo (`bottom:0`) según la card
- Vista mobile (≤600px): personajes centrados verticalmente, pegados a la derecha (`top:50% translateY(-50%) right:-5px width:100px`), texto con `padding-right:110px`
- Excepción Porkyburguer en mobile: `padding-right:20px`, personaje `width:85px top:-40px`
- Nubes redondeadas animadas (sin rect de tapa)
- WhatsApp configurado: `wa.me/573142173883`
- Elmer Fudd convertido de EPS→SVG y asignado a "La Cazadora de Elmer Gruñón"
- Tweety asignado a "Pío Pío Extreme" (antes tenía Daffy2)

## Archivos clave
```
C:\Dev\Toones food\
├── index.html          (~55KB)
└── assets/svg/
    ├── cloud.svg
    ├── chars/          (18 SVGs: bugs, bugs-running, chungus, daffy,
    │                    daffy2, elmer, foghorn, marvin, marvin2,
    │                    porky, roadrunner, roadrunner2, speedy,
    │                    sylvester, sylvester2, taz, tweety, yosemite)
```

## Next Step
Revisar vista mobile con screenshots nuevas — los ajustes de personajes en mobile quedaron pendientes de validación visual. Tomar screenshots con zoom al 150% en el navegador o usar la herramienta de recorte para capturar solo una sección (evitar imágenes >2000px).

## Blockers / Open Questions
- Screenshots mobile superan 2000px y el modelo las rechaza — usar recorte de pantalla o reducir resolución
- Animación flip recién agregada, no confirmada visualmente
- Vista desktop pendiente de verificación tras últimos cambios mobile

## Categorías y personajes asignados
| Card | Personaje | SVG |
|------|-----------|-----|
| La Piolín | Tweety | tweety.svg |
| La Cazadora de Elmer Gruñón | Elmer Fudd | elmer.svg |
| El Gran Banquete de Porky | Porky Pig | porky.svg |
| La Porkyburguer | Big Chungus | chungus.svg |
| Taz-Explosiva | Taz | taz.svg |
| Pato Chiflado | Daffy Duck | daffy.svg |
| La Correcaminos (hamb.) | Road Runner | roadrunner2.svg |
| Conejo Cruch | Bugs Running | bugs-running.svg |
| Taz's Tornado | Taz | taz.svg |
| Lindo Gatito | Sylvester | sylvester.svg |
| El Martillazo de Marvin | Marvin | marvin.svg |
| Pío Pío Extreme | Tweety | tweety.svg |
| Criollo | Foghorn Leghorn | foghorn.svg |
| La Correcaminos (mazorca) | Road Runner | roadrunner.svg |
| El Botín de San Bigotes | Sylvester 2 | sylvester2.svg |
| El Torbellino de Taz's | Taz | taz.svg |
| Bony Pinchos | Speedy Gonzales | speedy.svg |
