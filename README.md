# Drive-insight


## Overview
We present a debugging and analyzing tool for black-box end-to-end autonomous driving models.
<img width="780" alt="image" src="https://github.com/user-attachments/assets/e80cb9be-f256-41dd-a396-b3ee9d135cfa">


## Evaluation

Closed-loop evaluation on the Town05 Long & Short benchmarks. Our method achieve a
competitive driving score while also achieving the highest route completion. The sign * denotes that
we exclude data from town05 in the training set.


|Method|Modality|Reference|Training frames|Town05 Long DS|Town05 Long RC | Town05 Short DS| Town05 Short RC|
|---|---|---|---|---|---|---|---|
LBC| C | CoRL 20 | 150K | 12.3 | 31.9 | 31.0 | 55.0
Transfuser| C+L | TPAMI 22 | 150K | 31.0 | 47.5 | 54.5 | 78.4
ST-P3 | C | ECCV 22 | 150K | 11.5 | 83.2 | 55.1 | 86.7
VAD | C | ICCV 23 | 3.0M | 30.3 | 75.2 | 64.3 | 87.3
ThinkTwice | C+L | CVPR 23 | 2.2M | 70.9 | 95.5 | - | -
MILE | C | NeurIPS 22 | 2.9M | 61.1 | 97.4 | - | -
Interfuser | C | CoRL 22 | 3.0M | 68.3 | 95.0 | 94.9 | 95.2
DriveAdapter | C+L | ICCV 23 | 2.0M | **71.9** | 97.3 | - | -
Ours | C+L | - | 1.8M | 66.6 | **100.0** | **95.3** | **99.2**
Ours* | C+L | - | 1.5M | 64.4 | **100.0** | 93.2 | 95.8
