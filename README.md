# Dynamic_RR
  - [Abstract](#abstract)
  - [Hypothesis](#hypothesis)
  - [CPU Utiliation](#cpu-utilization)
  - [Algorithm](#algorithm)
  - [Experiment](#experiment)
    - [Case 1](#case-1)
    - [Case 2](#case-2)
    - [Case 3](#case-3)
  - [Reference](#reference)

## Abstract
> 범용 스케줄러-선점형 OS Scheduler 중 하나인 Round Robin(RR)을 변형한 알고리즘을 구현하였다. 기존의 Round Robin은 초기 Time Quantum을 설정하여 프로세스들을 스케줄하지만 Proposed Round Robin(Dynamic RR)은 Time Quantum을 유동적으로 변경한다는 차이점이 있다.<br>
> Dynamic Round Robin은 _Waiting Time_, _Turnaround Time_ 측면에서 향상된 성능을 보였고 전체적인 _Response Time_ 측면에서는 기존 RR보다 낮은 성능을 보였다.

## Hypothesis
- 프로세스들을 foreground와 background로 나누지 않고 전부 상호작용적(interactive)으로 작동하는 foreground processes라고 가정
- 각 프로세스에 대한 Arrival Time, Burst Time 제공
---
## CPU Utilization
<img src='./img/cpu_util.png'>

---
## Algorithm
<p align="center"><img src="./img/algorithm.png" width="80%" height="80%">

---
## Experiment
### Case 1
|ID|Arrival Time|Burst Time|
|:-----:|:---:|:---:|
|P1|40|10|
|P2|0|1|
|P3|43|3|
|P4|19|8|
|P5|44|1|
|P6|23|4|
|P7|50|11|
|P8|15|1|
|P9|3|6|
|P10|26|11|

<p align="center"><img src="./img/case1/case1.png" width="80%" height="80%">

<img src="./img/case1/case1_rr_result.png" width="45%" height="45%">
<img src="./img/case1/case1_pr_result.png" width="45%" height="45%" align="right">

<img src="./img/case1/case1_rr.png" width="45%" height="45%">
<img src="./img/case1/case1_pr.png" width="45%" height="45%" align="right">

***

### Case 2
|ID|Arrival Time|Burst Time|
|:-----:|:---:|:---:|
|P1|8|12|
|P2|9|11|
|P3|46|1|
|P4|12|14|
|P5|19|7|
|P6|1|8|
|P7|28|4|
|P8|2|14|
|P9|43|5|
|P10|2|6|

<p align="center"><img src="./img/case2/case2.png" width="80%" height="80%">

<img src="./img/case2/case2_rr_result.png" width="45%" height="45%">
<img src="./img/case2/case2_pr_result.png" width="45%" height="45%" align="right">

<img src="./img/case2/case2_rr.png" width="45%" height="45%">
<img src="./img/case2/case2_pr.png" width="45%" height="45%" align="right">

***

### Case 3
<p align="center"><img src="./img/case3/case3.png" width="80%" height="80%">

<img src="./img/case3/case3_rr_result.png" width="45%" height="45%">
<img src="./img/case3/case3_pr_result.png" width="45%" height="45%" align="right">

<img src="./img/case3/case3_rr.png" width="45%" height="45%">
<img src="./img/case3/case3_pr.png" width="45%" height="45%" align="right">

---
## Reference
- A New Round Robin Based Scheduling Algorithm for Operating Systems: Dynamic Quantum Using the Mean Average-[arxiv.org](https://arxiv.org/pdf/1111.5348.pdf)
- [CPU Scheduling](http://uclab.khu.ac.kr/lectures/2006_1_os/os-ch06.pdf)