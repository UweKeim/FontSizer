# FontSizer configurable environment step

## Context
- Datum: 2026-02-27
- Ziel: Fork von `madskristensen/FontSizer` zu `UweKeim/FontSizer`, Environment-Schrittweite konfigurierbar machen, lokal baubares VSIX erzeugen.

## Plan (persistiert)
1. Fork erzeugen und lokalen Checkout unter `C:\P\FontSizer-UweFork` erstellen.
2. Extension als separat installierbare Variante umstellen (eigene VSIX-/Package-ID).
3. Neue Option in Visual Studio für Environment-Schrittweite einführen (Default 1).
4. Environment-Commands auf Option umstellen und robust gegen Unterlauf machen.
5. Build/Packaging prüfen und VSIX-Artefakt bereitstellen.
6. Änderungen committen und auf Fork pushen.

## Fortschritt
- [x] Fork erstellt: `UweKeim/FontSizer`
- [x] Lokaler Branch erstellt: `feature/configurable-environment-step`
- [x] Codeänderungen umgesetzt
- [x] Build erfolgreich verifiziert
- [x] Commit + Push abgeschlossen

## Entscheidungen
- Separate Installation statt Überschreiben der Original-Extension.
- Konfigurierbare Schrittweite statt Hardcode.
- Default für Environment-Schrittweite: `1`.
- Wertebereich: `1..10`.

## Offene Punkte
- Build muss erfolgreich durchlaufen.
- VSIX-Artefaktpfad nach Build bestätigen.
- Push per PAT abschließen.