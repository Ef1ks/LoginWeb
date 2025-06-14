# LoginWeb - Prosty Formularz Logowania

Ten projekt przedstawia responsywny formularz logowania i rejestracji, zbudowany w oparciu o podstawowe technologie webowe: HTML i CSS. Strona zawiera również nawigację, breadcrumbs (okruszki chleba) oraz integrację z Google reCAPTCHA v2 dla zwiększenia bezpieczeństwa.

---

## Technologie

Projekt został zrealizowany przy użyciu:

* **HTML5:** Do strukturyzowania treści strony.
* **CSS3:** Do stylizacji i zapewnienia responsywności układu.
* **Google reCAPTCHA v2:** Do ochrony formularza przed spamem i automatycznymi botami.

---

## Główne Cechy

* **Responsywny Design:** Układ strony dostosowuje się do różnych rozmiarów ekranów, zapewniając dobre wrażenia użytkownika zarówno na komputerach stacjonarnych, jak i urządzeniach mobilnych.
* **Formularz Logowania:** Prosty formularz do wprowadzania nazwy użytkownika, adresu e-mail i hasła.
* **Sekcja Rejestracji:** Zachęcająca sekcja dla nowych użytkowników z przyciskiem do rejestracji.
* **Nawigacja i Breadcrumbs:** Intuicyjna nawigacja główna oraz ścieżka okruszków chleba (breadcrumbs) ułatwiająca orientację na stronie.
* **Integracja reCAPTCHA:** Wbudowana weryfikacja reCAPTCHA v2 w formularzu logowania.
* **Animacje CSS:** Płynne animacje elementów interfejsu (np. przycisków, panelu rejestracji).

---

## Instalacja i Uruchomienie

Aby uruchomić projekt lokalnie, wykonaj następujące kroki:

1.  **Sklonuj repozytorium:**
    ```bash
    git clone https://github.com/Ef1ks/LoginWeb.git
    ```
2.  **Przejdź do katalogu projektu:**
    ```bash
    cd LoginWeb
    ```
3.  **Otwórz plik `index.html`** w swojej przeglądarce internetowej.

---

## Konfiguracja Google reCAPTCHA v2

Aby reCAPTCHA działała poprawnie, musisz podmienić klucz witryny (`data-sitekey`) na swój własny, uzyskany z Google.

1.  **Uzyskaj klucze reCAPTCHA:**
    * Przejdź na stronę [Google reCAPTCHA](https://www.google.com/recaptcha/admin/create).
    * Zaloguj się na swoje konto Google.
    * Zarejestruj nową witrynę. Wybierz **"reCAPTCHA v2"** i typ **"Pole wyboru „Nie jestem robotem”"**.
    * W polu "Domeny" **musisz dodać `127.0.0.1`**, aby reCAPTCHA działała poprawnie podczas testowania lokalnego. Możesz również dodać `localhost` oraz docelową domenę, jeśli planujesz wdrożenie projektu.
    * Po rejestracji otrzymasz **Klucz witryny** (Site Key) i Klucz tajny (Secret Key).

2.  **Podmień `data-sitekey` w pliku `index.html`:**
    * Otwórz plik `index.html`.
    * Znajdź linię zawierającą `data-sitekey`:
        ```html
        <div class="g-recaptcha" data-sitekey="6Lc-Rl0rAAAAAI5AECHRu_iIPOz1LyPu6HpL9he9" required></div>
        ```
    * Zastąp wartość `6Lc-Rl0rAAAAAI5AECHRu_iIPOz1LyPu6HpL9he9` swoim **Kluczem witryny**.

---

## Autor

Ef1ks

---

