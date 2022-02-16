# hse_hw1_meth
# Colab
```
https://colab.research.google.com/drive/1zM28Fag5K8VMNKs5O2Ojy2CG8dN3D1_8?usp=sharing
```
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
# SRR3824222
![Image](images/HEATMAP.png)
