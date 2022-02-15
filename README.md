# hse_hw1_meth
# Число ридов
BS-Seq | 11347700-11367700 | 40185800-40195800 
--- | --- | ---
SRR5836473 | 1090 | 464
SRR3824222 | 2328 | 1062
SRR5836475 | 1456 | 630
# BASH-скрипт
```
!ls *pe.bam | xargs -P 4 -tI{} deduplicate_bismark  --bam  --paired  -o s_{} {}
```
