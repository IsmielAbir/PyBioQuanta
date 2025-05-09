# PyBioQuanta

**PyBioQuanta** is a lightweight Python package offering 6 essential bioinformatics utilities.  
It is designed for quick sequence operations, small analyses, and everyday bioinformatics tasks.

---

## Features

- **FASTA Reader**: Parse FASTA files into Python dictionaries.
- **Reverse Complement**: Get the reverse complement of DNA or RNA sequences.
- **DNA Translator**: Translate DNA sequences into protein.
- **GC Content Calculator**: Calculate GC percentage of a sequence.
- **Motif Finder**: Find positions of motifs (subsequences) inside sequences.
- **Random DNA Generator**: Create random DNA sequences of desired length.

---

## Installation

You can install PyBioQuanta via pip:

```bash
pip install PyBioQuanta
```


# Usage
## 1. FASTA Reader
```bash
from PyBioQuanta import read_fasta

sequences = read_fasta("example.fasta")
print(sequences)
```

## 2. Reverse Complement

```bash
from PyBioQuanta import reverse_complement

seq = "ATCG"
rc = reverse_complement(seq)
print(rc)
```

## 3. DNA Translator

```bash
from PyBioQuanta import translate_dna

dna_seq = "ATGGCCATTGTAATGGGCCGCTGAAAGGGTGCCCGATAG"
protein = translate_dna(dna_seq)
print(protein)
```


## 4. GC Content Calculator

```bash
from PyBioQuanta import gc_content

seq = "ATGCGC"
gc_percentage = gc_content(seq)
print(f"GC Content: {gc_percentage:.2f}%")

```



## 5. Motif Finder

```bash
from PyBioQuanta import find_motif

seq = "ATGCGCGTAGCGC"
motif = "GCG"
positions = find_motif(seq, motif)
print(positions)
```


## 6. Random DNA Generator

```bash
from PyBioQuanta import generate_random_dna

random_seq = generate_random_dna(50)
print(random_seq)


```
