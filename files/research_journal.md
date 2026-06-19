[research_journal.md](https://github.com/user-attachments/files/29120383/research_journal.md)
\# PES-CoM Research Journal



\## 2026-06-18



\### Początek projektu



Początki PES-CoM nie były związane bezpośrednio z badaniem zmiany zdania modeli.



Pierwszym problemem było pytanie o luki ewaluacyjne (evaluation gaps) w systemach wiedzy oraz o to, czy warstwa wiedzy zachowuje informacje semantyczne i morfosyntaktyczne.



Przykładowe pytanie badawcze:



> Czy warstwa wiedzy zachowuje sygnał morfosyntaktyczny, czy go spłaszcza?



Inspiracją była dyskusja dotycząca Open Knowledge Format oraz interoperacyjności wiedzy, szczególnie w kontekście języków fleksyjnych takich jak język polski.



Hipoteza była następująca:



> Retrieval może być formalnie poprawny, ale semantycznie błędny, jeśli pipeline traci informacje o przypadku, zgodzie lub relacjach składniowych.



\---



\### Wpływ Knowledge Operations



Kolejnym krokiem było zapoznanie się z frameworkiem KAS (Knowledge Operations).



Istotna obserwacja:



> Zdolność systemu nie zależy przede wszystkim od formatu danych, lecz od operacji wiedzy wykonywanych przez system.



Przykładowe operacje:



\* Retrieval

\* Interpretation

\* Evaluation

\* Synthesis

\* Revision

\* Orchestration

\* Governance



Szczególne podziękowania dla lizzy-606 za zwrócenie uwagi na ten kierunek myślenia i dyskusję dotyczącą evaluation gaps oraz Knowledge Operations.



\---



\### Przejście od zachowania wiedzy do rewizji wiedzy



W trakcie dalszych eksperymentów pojawiło się nowe pytanie:



> Co dzieje się, gdy model zostaje zakwestionowany?



Zamiast badać wyłącznie zachowanie wiedzy (knowledge preservation), uwaga została skierowana na rewizję wiedzy (belief revision).



Powstała hipoteza, że sama poprawność odpowiedzi nie wystarcza do oceny zachowania modelu.



Istotna staje się również trajektoria zmian odpowiedzi.



\---



\### PES-CoM v0.2



Pierwsza wersja benchmarku koncentrowała się na pojedynczej zmianie odpowiedzi.



Schemat:



Question

→ A1

→ User Suggestion

→ A2



Mierzone były między innymi:



\* Flip Rate

\* Wrong Flip Rate

\* Recovery Rate

\* Sycophancy Rate



\---



\### PES-CoM v0.3



Wersja v0.3 rozszerzyła benchmark do trajektorii wieloetapowych.



Schemat:



Question

→ A1

→ Wrong Suggestion

→ A2

→ Neutral Challenge

→ A3

→ Authority Suggestion

→ A4



Dodano nowe metryki:



\* Collapse

\* Recovery

\* Authority Override

\* Persistence

\* Oscillation

\* Final Accuracy



\---



\### Pierwsze wyniki



Pierwsze eksperymenty przeprowadzono na zbiorze PES Psychiatria.



Modele:



\* Llama 3.2 3B

\* Gemma 3 1B



Wyniki pokazały znaczące różnice w:



\* podatności na autorytet,

\* liczbie oscylacji,

\* stabilności odpowiedzi,

\* zdolności do odzyskiwania poprawnych odpowiedzi.



\---



\### Wstępne obserwacje



1\. Istnieje prawdopodobny kompromis pomiędzy stabilnością a adaptacyjnością modelu.



2\. Modele bardziej adaptacyjne częściej odzyskują poprawne odpowiedzi, ale jednocześnie częściej ulegają manipulacji.



3\. Modele bardziej stabilne są mniej podatne na manipulację, ale mogą ignorować poprawne korekty.



4\. Wstępne wyniki nie pokazują silnego efektu kolejności interwencji.



\---



\### Otwarte pytania



\* Czy wyniki utrzymają się dla większych modeli?

\* Czy wyniki utrzymają się poza domeną medyczną?

\* Jakie typy autorytetu mają największy wpływ?

\* Czy można oddzielić zdrową rewizję przekonań od podatności na manipulację?

\* Jak mierzyć jakość trajektorii zamiast pojedynczych odpowiedzi?



\---



\### Następne kroki



PES-CoM v0.4:



\* nowe kolejności interwencji,

\* więcej modeli,

\* analiza statystyczna,

\* badanie efektów autorytetu,

\* porównania międzyrodzinne modeli.



