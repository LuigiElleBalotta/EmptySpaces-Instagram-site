# Empty Spaces (sito cifrato)

Questo repository contiene solo un file HTML **cifrato**: senza la password non è leggibile. Viene generato e ripubblicato automaticamente dal repository privato a ogni commit. **Non modificare nulla qui**: la prossima pubblicazione sovrascrive tutto.

## Chat con Gibby (avvio, sul PC di Luigi)
La chat del sito (pulsante **Gibby**) funziona solo se sul PC di Luigi sono attivi Tailscale e il ponte. Dalla cartella del repository **privato** `EmptySpaces-Instagram`:

```powershell
# avvio automatico a ogni accesso a Windows (una volta sola):
powershell -ExecutionPolicy Bypass -File ops/bridge/install_autostart.ps1

# oppure un solo comando a mano:
powershell -ExecutionPolicy Bypass -File ops/bridge/start_gibby.ps1

# oppure proprio a mano:
python ops/bridge/bridge.py

# per fermare:
powershell -File ops/bridge/stop_gibby.ps1
```
Dettagli e sicurezza: `docs/CHAT.md` nel repository privato. Se la chat mostra "Gibby è offline", il PC, Tailscale o il ponte sono spenti.
