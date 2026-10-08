# RetroXam

**Lista curada de los mejores juegos retro — prioridad español — para PC/Android (RetroBat y similares).**

35 sistemas, ~4.400 juegos, en formato **JSONL oficial** (el mismo que usan las apps tipo Arley4d):
cada línea describe un juego con sus URLs de descarga, tamaño y metadatos.

## Qué hay dentro

- **35 sistemas**: NES, SNES, GB/GBC/GBA, N64, Mega Drive/CD/32X, PSX, PS2, PS3, PSP, PSVita,
  Saturn, Dreamcast, GameCube, Wii, WiiU, Switch, 3DS, NDS, Xbox, Xbox 360, Neo Geo,
  CPS1/2/3, FBNeo, Naomi, Naomi2, Atomiswave, Model 2/3, OpenBOR…
- **~4.400 juegos** seleccionados por rankings reales (IGN, GamesRadar, Retro Sanctuary,
  Metacritic…) y **priorizando versiones con español** cuando existen.
- Formato **`.jsonl`** con finales de línea CRLF (compatible byte a byte con el formato oficial).

## Cómo usarla

### PC (RetroBat u otros frontends)
```bash
python crear_fakeroms.py --repo https://github.com/servixam-max/RetroXam --out C:\RetroBat\ROMs --clean
```
Genera fake roms (~100 B) — la app interceptor descarga el juego real al lanzarlo.

### Android
Instala **RetroXam FakeROMs** (APK) y apunta al repo; la app crea las fake roms y
un zip compartible para el dispositivo.

## Sistema "fake rom"
Los archivos pesan ~100 bytes: contienen la URL del juego real (`URL *Size=...`).
Al lanzarlos, el descargador (Arley4dBypassPC en PC / app en Android) descarga y ejecuta.

## Repos relacionados
- **RetroXamVita** — la versión reducida para PS Vita (16 sistemas emulables).
- **RetroXamTools** — herramientas PC (fakeroms, descarga para Vita).
