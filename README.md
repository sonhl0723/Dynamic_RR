# Dynamic_RR

## Hypothesis
- 프로세스들을 foreground와 background로 나누지 않고 전부 상호작용적(interactive)으로 작동하는 foreground processes라고 가정
- 각 프로세스에 대한 Arrival Time, Burst Time 제공
---
## CPU Utilization
<img src='./img/cpu_util.png'>
<!-- - $CPU$ $utilization$(%) $=$ ($\frac{BUSY Time} {TOTAL Time}$) $*$ $100$ ...(1)
- $TOTAL$ $Time$= $IDLE$ $Time$ $+$ $BUSY$ $Time$ ...(2)
- $BUSY$ $Time$ $=$ $TOTAL$ $Time$ $-$ $IDLE$ $Time$ ...(3)

<!-- $$
CPU utilization = (\frac{BUSY Time} {TOTAL Time}) * 100 = 1 - (\frac{IDLE Time} {TOTAL Time}) * 100
$$  -->
---
## Algorithm
<p align="center"><img src="./img/algorithm.png" width="80%" height="80%">

---
## Experiment
### Case 1
<p align="center"><img src="./img/case1/case1.png" width="80%" height="80%">

<img src="./img/case1/case1_rr.png" width="45%" height="45%">
<img src="./img/case1/case1_pr.png" width="45%" height="45%" align="right">

### Case 2

### Case 3