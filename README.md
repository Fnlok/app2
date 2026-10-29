# Builds Locas LoL (app de escritorio)

App para Windows, macOS y Linux. No usa IA, claves ni servidores: todo se calcula en tu equipo con los datos oficiales de Riot (Data Dragon), que se descargan al abrir la app y se actualizan solos con cada parche. Necesita internet.

## Qué incluye
- Los 173 campeones con su ficha oficial: splash, habilidades, historia, aspectos y consejos de Riot para jugar con ellos y contra ellos.
- Builds raras: 3 por campeón (y más a pedido) con orden de compra, botas, runas, qué banear y guía del matchup.
- Equipos exóticos: sortea cientos de equipos, puntúa su sinergia con los datos de Riot y arma los campeones fuera de su línea habitual. Equipo completo, botlane o mid y jungla.
- Modo «Caos puro», ruleta, copiar equipo, favoritos y sonidos (con botón para silenciarlos).

## Probarla en tu equipo
Necesitas Node.js 20 o superior.

    npm install
    npm start

## Crear los instaladores
    npm run dist:win      # Windows (.exe)
    npm run dist:mac      # macOS (.dmg, Intel y Apple Silicon)
    npm run dist:linux    # Linux (.AppImage y .deb)

Los archivos quedan en `dist/`. Para crear los tres sin tener los tres sistemas, sube el proyecto a GitHub y ejecuta «Construir instaladores» en la pestaña Actions.

## Avisos al instalar
Los instaladores no están firmados. Windows puede mostrar SmartScreen («Más información» y «Ejecutar de todos modos»). En macOS, abre la app con clic derecho y «Abrir» la primera vez.

## Icono
Usa el icono por defecto de Electron. Para uno propio crea `build/icon.png` (512x512 o más) y vuelve a construir.
