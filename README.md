# hse_hw1_meth
# Число ридов
BS-Seq | 11347700-11367700 | 40185800-40195800 | deduplication % 
--- | --- | --- | ---
SRR5836473 | 1090 | 464 | 81.69
SRR3824222 | 2328 | 1062 | 97.08
SRR5836475 | 1456 | 630 | 90.92
# BASH-скрипт
```
!ls *pe.bam | xargs -P 4 -tI{} deduplicate_bismark  --bam  --paired  -o s_{} {}
```
