# Dynamic_RR

## Hypothesis
- 프로세스들을 foreground와 background로 나누지 않고 전부 상호작용적(interactive)으로 작동하는 foreground processes라고 가정
- 각 프로세스에 대한 Arrival Time, Burst Time 제공
---
## CPU Utilization
- $CPU$ $utilization$(%) $=$ ($\frac{BUSY Time} {TOTAL Time}$) $*$ $100$ ...(1)
- $TOTAL$ $Time$= $IDLE$ $Time$ $+$ $BUSY$ $Time$ ...(2)
- $BUSY$ $Time$ $=$ $TOTAL$ $Time$ $-$ $IDLE$ $Time$ ...(3)

$$
CPU utilization = (\frac{BUSY Time} {TOTAL Time}) * 100 = 1 - (\frac{IDLE Time} {TOTAL Time}) * 100
$$
---
## Algorithm
<center><img src="./img/algorithm.png" width="80%" height="80%"></center>

---
## Experiment
### Case 1
<div>
    <center>
    <img src="./img/case1/case1.png" width="80%" height="80%">
    </center>

<div style="width:250px; height:250px; border:1px solid red; float:left;">
<img src="./img/case1/case1_rr.png" width="100%" height="100%">
</div>

<div style="width:250px; height:250px; border:1px solid green; float:left;">
<img src="./img/case1/case1_pr.png" width="100%" height="100%">
</div>
</div>

### Case 2

### Case 3