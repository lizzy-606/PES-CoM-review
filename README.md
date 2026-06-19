# PES-CoM — zewnętrzna recenzja analityczna

Repozytorium zawiera niezależną analizę projektu **PES-CoM (Change of Mind Benchmark)** autorstwa Piotra Styły.

**Projekt oryginalny:** https://github.com/PiotrStyla/PES-CoM/tree/v0.3-multiturn  
**Recenzja:** lizzy-606

---

## Struktura repozytorium

```
README.md                        ← ten plik
files/                           ← pliki źródłowe z repo PES-CoM (v0.3-multiturn)
  README.md
  glossary.md
  multiturn_results.md
  multiturn_design.md
  evaluator_test_cases.md
  research_journal.md
analysis/
  PES-CoM_analiza.md             ← notatka analityczna
```

---

## O analizie

Analiza przeprowadzona w trzech etapach:

**Etap 1** — na podstawie plików z repozytorium (bez datasetu).  
**Etap 2** — po wglądzie w dataset (`pes_com_psychiatria_100_v02.jsonl`).  
**Etap 3** — dane Qwen 3 4B (`qwen3_4b_wrong.jsonl`) jako osobna kategoria problemu.

Struktura etapów jest celowa: pokazuje, które wnioski są widoczne już na poziomie architektury projektu, a które wymagają wglądu w dane surowe.

---

## Kontekst

Recenzja powstała w ramach dyskusji w kanale `#benchmarki`. Uwagi dotyczą metodologii, definicji metryk i interpretowalności wyników — nie są krytyką projektu jako całości. Projekt ma solidne podstawy i kilka nieoczywistych mocnych stron, które również zostały odnotowane.
