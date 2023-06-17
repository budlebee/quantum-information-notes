

주로 밴드계산 하는 세가지방법

1. Tight binding
2. Augmented Plane Wave (APW) method -> LAPW -> FLAPW
3. Pseudopotentials -> ab initio pesudopotentials

Tight binding : 이해하기 직관적이고 계산량이 적다

APW : 결과가 정확하지만 계산량이 많다. 

ab initio : 계산이 빠르다. 하지만 그래서 실험결과와 비교하며 체크가 필요함. 재료공학, 기계공학에서 많이 씀.

요즘 트랜지스터는 스케일이 나노단위로 줄어들었고, 컴퓨터 하드웨어 계산능력이 좋아져서, 트랜지스터에 있는 모든 전자들을 고려하는 ab initio 계산을 최근 시도하는 듯.

계산량은 원자수 $N^3$ 에 비례함. 

Bloch theorem : manybody 를 single particle picture 로 바꿔서 푼 것. 싱글 라인 밴드 그림도 싱글 파티클에 대한 방정식을 풀어서 나온 결과인 것. LDA 나 DMFT 의 결과는 밴드 그림이 두께가 있어서 두께가 늘어났다 줄어났다 그럼. 이런건 manybody 에 더 가깝게 푼 것.

$$
(-\frac{\hbar^2}{2m}\nabla^2 + U(r))\psi_k(r) = \epsilon(k)\psi_k(r)
$$

여기서 $\nabla^2$ 부분은 바뀌지 않고, 물성이 들어가는 부분은 $U(r)$ 부분임. 이때 이 방정식은 spin orbit coupling 을 고려하지 않은 식임. 

싱글파티클 방정식은 코어 일렉트론이나 valence 일렉트론이나 같은 포텐셜 U 를 씀. 이게 문제점임. 왜냐면 valence electron 은 코어 전자와 다른 valence 전자들이 만드는 screening + 파울리 exclusive principle 로 인해 core 상태로 갈 수 없음 으로 core 가 만드는 potential 을 느끼는게 작다. 

Na 의 원자의 경우, 고체상태로 있나 원자상태로 있나 core electron 들은 그 차이를 별로 못 느낀다. 
고전적으로, 양전하 주위를 음전하가 회전할때 포텐셜 에너지는 운동에너지의 -2 배 정도를 가진다. 그래서 운동에너지가 증가하면 포텐셜 에너지가 -2배 줄어들어서 결과적으로 전체 에너지가 줄어듬. W-S cell 에 cellular 방법을 쓴 결과도 비슷하게 나옴. 고체를 이룬 전자의 운동에너지는 증가하는데 포텐셜 에너지가 더 많이 줄어들어서 결과적으로 전체 에너지가 줄어듬.