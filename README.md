## Przygotowanie zadań do egzaminu ustnego

Prof. Bogdan udostępnił nam pytania na egzamin.
Ich kopia znajduję się w tym [arkuszu.](https://docs.google.com/spreadsheets/d/1F0lyvLjYyfNODudUN2nthQ9vvAZUmfRzZxIS6NAlk0s/edit#gid=0)

### Aby dodać opracowanie:
1. Odznacz się w arkuszu w kolumnie `kto opracuje?`.
1. Sklonuj to repozytorium.
1. Dopisz rozwiązanie zadania w odpowiednim miejscu w pliku `opracowanie.tex`.
1. Upewnij się, że plik `pdf` się kompiluje.
1. Przekaż zmiany do repozytorium. Można to zrobić na 2 sposoby:
    - Wykonaj commita i utwórz `pull request` **albo** (jeśli nie chcesz lub nie wiesz jak to zrobić)
    - Wykonaj komendę `git diff origin/HEAD` i prześlij to, co ona zwróci do organizatora.
1. Oznacz w arkuszu, że punkt został zrobiony.

Komenda `git diff` pokazuje, co zostało zmienione i można na jej podstawie szybko
dodać zmiany w scentralizowany sposób, bez konfliktów gita.

### Usterki
Jeśli wydaje Ci się, że dodana odpowiedź jest niepełna lub zawiera błąd,
skontaktuj się z autorem odpowiedzi lub napisz to w komórce `uwagi` w arkuszu.


--------

W przypadku przesyłanie wyniku komendy `git diff`,
powinna ona wyglądać mniej więcej tak jak poniżej.
``` diff
diff --git a/opracowanie.tex b/opracowanie.tex
index 2e6a112..c631bc1 100644
--- a/opracowanie.tex
+++ b/opracowanie.tex
@@ -77,7 +77,9 @@ Jak definiuje się własność Markowa procesu stochastycznego?
 Jakie postulaty spełnia macierz przejścia łańcucha Markowa?
 \end{pytanie}
 \begin{odpowiedź}
-    % tu zamieść odpowiedź
+    To jest odpowiedź na pytanie powyżej.
+    Tu jest druga linijka.
+    Tu jest trzecia.
 \end{odpowiedź}
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

```

Przesyłamy **cały** zwrócony tekst, czyli
``` txt
diff --git a/opracowanie.tex b/opracowanie.tex
index 2e6a112..c631bc1 100644
--- a/opracowanie.tex
+++ b/opracowanie.tex
@@ -77,7 +77,9 @@ Jak definiuje się własność Markowa procesu stochastycznego?
 Jakie postulaty spełnia macierz przejścia łańcucha Markowa?
 \end{pytanie}
 \begin{odpowiedź}
-    % tu zamieść odpowiedź
+    To jest odpowiedź na pytanie powyżej.
+    Tu jest druga linijka.
+    Tu jest trzecia.
 \end{odpowiedź}
 %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

```

Dobrą metodą upewnienia się, że cały tekst został skopiowany jest wykonanie
`git diff origin/HEAD > zmiany.diff` i przesłanie powstałego pliku `zminay.diff`.
