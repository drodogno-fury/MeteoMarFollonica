# MeteoMar Follonica - App Android

App meteo per il Golfo di Follonica con dati in tempo reale.

## Fonti Dati (100% Gratuito - COSTO ZERO)
| Fonte | Dato | API Key? |
|---|---|---|
| Open-Meteo (ECMWF/GFS) | temp, vento, pressione, pioggia | NO |
| Open-Meteo Marine | onde, swell, periodo | NO |
| Windy embed | mappa vento animata | NO |
| MeteoAM | link ufficiale Aeronautica | NO |
| 3BMeteo / iLMeteo | link previsioni locali | NO |

## Come aprire in Android Studio
1. Installa **Android Studio** (Hedgehog 2023.1+)
2. File -> Open -> seleziona la cartella `MeteoMarFollonica`
3. Attendi sync Gradle (serve connessione internet)
4. Collega un device Android o avvia emulatore
5. Premi Run (triangolo verde)

## Requisiti
- Android min SDK 24 (Android 7.0+)
- Connessione internet per i dati live
- Android Studio 2023.1+

## Struttura progetto
- `app/src/main/assets/index.html` -> tutta l'UI e la logica dati
- `app/src/main/java/.../MainActivity.kt` -> Activity con WebView
- Dati fetched in tempo reale da API gratuite, nessun backend
