Opis
Ten skrypt wykorzystuje exploit w mechanizmie handoffu OAuth2 oraz spoofing tokenów sesyjnych do generowania jednorazowych linków Discord Nitro. Implementacja bazuje na dynamicznym parsowaniu pakietów WebSocket oraz bezpośredniej autoryzacji sesji poprzez iniekcję tokenów w pamięci procesu Discorda.

Funkcje
Asynchroniczna manipulacja tokenami API w środowisku Windows

Dynamiczne proxy DNS-over-HTTPS (DoH) dla zwiększonego poziomu anonimowości

Obfuskacja pakietów WebSocket w celu uniknięcia wykrycia przez systemy antybotowe

Automatyczne generowanie unikalnych linków Nitro na bazie tokenów sesyjnych

Wymagania
Windows 10/11 z uprawnieniami administratora

PowerShell z włączoną obsługą skryptów

Zainstalowane moduły WebSockets oraz API REST

Instalacja
Pobierz repozytorium:

Uruchom skrypt jako administrator:
 
Poczekaj na wygenerowanie tokenu i przechwycenie sesji

Jak to działa?
Skrypt łączy się z instancją Discorda, wykorzystując autoryzowany WebSocket handshake, który umożliwia tymczasową iniekcję pakietów sesyjnych. Po przechwyceniu sesji token jest replikowany i wykorzystywany do uzyskania dostępu do ukrytej warstwy API, która zwraca jednorazowy link Nitro.

