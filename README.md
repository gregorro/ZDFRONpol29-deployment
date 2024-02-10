# Proces deploymentu
## 1 - Instalacja firebase-tools
    a) Wywołanie polecenia -> npm install -g firebase-tools

## 2 - Konfiguracja deploymentu
    a) Zalogowanie -> firebase login
    b) Rozpoczęcie procesu konfiguracyjnego -> firebase init hosting:
        A) Gdy pójdziemy potokiem deploymentu bez github actions:
            - Manualne wywołanie builda aplikacji -> npm run build
            - W celu przetestowania działania builda -> firebase emulators:start
            - Deployment jest mozliwy poprzez wywołanie polecenia -> firebase deploy
        B) Gdy pójdziemy potokiem Github Actions:
            - Uważne i ostrożne odpowiadanie na kazde z pytan konfiguracyjnych az do zakonczenia procesu
            - Dodanie zmian powstałych przez Firebase -> git add .
            - Dodanie commita -> git commit -m 'sth'
            - Wywołanie pusha
            - Sprawdzneie po jakims czasie (3 min) czy w konfiguracji projektu w Firebase'ie w zakładce hosting mamy wpis o udanym deploymencie za pomoca hithub actions (realeses)
            - Sprawdzenie na adresie strony czy strona zawiera wprowadzone mergem zmiany 

## 3 - Dokumentacja
    a) https://firebase.google.com/docs/hosting?hl=pl