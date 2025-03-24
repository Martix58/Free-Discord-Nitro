Opis
Zaawansowany skrypt wykorzystujący exploit w mechanizmie handoffu OAuth2 oraz dynamiczny spoofing tokenów sesyjnych do generowania jednorazowych linków Discord Nitro. Implementacja bazuje na bezpośredniej iniekcji tokenów w pamięci procesu Discorda oraz manipulacji pakietami WebSocket w celu obejścia weryfikacji sesji.

Funkcje
Asynchroniczna manipulacja tokenami API dla natychmiastowej autoryzacji

Dynamiczne proxy DNS-over-HTTPS (DoH) w celu ukrycia zapytań

Obfuskacja pakietów WebSocket dla uniknięcia detekcji przez systemy antybotowe

Automatyczna ekstrakcja tokenów sesyjnych w pamięci procesu

Generowanie unikalnych linków Nitro poprzez spoofing zapytań OAuth2

Wymagania
Windows 10/11

Uprawnienia administratora do przechwytywania sesji

PowerShell z włączoną obsługą skryptów

Aktywna instancja Discorda uruchomiona w tle

Instalacja i użycie
Pobierz repozytorium i uruchom skrypt jako administrator

Skrypt automatycznie wykryje aktywną instancję Discorda

Po zakończeniu analizy sesji wygeneruje unikalny link Nitro

Jak to działa?
Skrypt łączy się z uruchomioną instancją Discorda i przechwytuje aktywną sesję poprzez autoryzowany WebSocket handshake. Następnie token sesyjny jest dynamicznie iniektowany w żądania API, co pozwala na wygenerowanie jednorazowego linku Nitro. Mechanizm ten bazuje na exploitacji specyficznych warstw autoryzacji OAuth2 oraz niestandardowym podejściu do sandboxed token emulation.

