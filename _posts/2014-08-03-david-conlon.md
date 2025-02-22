---
title:  "옥스포드대학 데이비드 콘론 교수"
date:   2014-08-03 22:55:00 +0900
tags: [그린타오정리,램지]
author: joonkyung
mathjax: true
---

> 편집자주: 서울에서 열릴 [2014 세계수학자대회](http://icm2014.org/)(ICM)를 기념하여, 조합수학 분야의 기조강연자 및 초청강연자들을 소개하는 글을 준비하였습니다. 이번 글은 2014년 8월 15일 오후 3시에 강연할 옥스포드 대학 [데이비드 콘론(David Conlon) 교수](https://www.its.caltech.edu/~dconlon/)에 대해, 그의 첫 박사과정 지도학생인 [이준경](https://sites.google.com/site/joonkyungleemaths/) 학생이 소개하는 글을 싣습니다.

<figure>
<img src="/assets/images/conlon.jpg" alt="David Conlon"/>
<figcaption>David Conlon</figcaption>
</figure>

1982년 태어난 콘론 교수는 아일랜드 출신으로, 필즈 메달 수상자인 [Timothy Gowers](https://en.wikipedia.org/wiki/Timothy_Gowers) 교수의 지도를 받고 캠브리지 대학에서 박사를 받았습니다. 콘론 교수의 전문 분야는 [극단 조합론(extremal combinatorics)](https://en.wikipedia.org/wiki/Extremal_combinatorics)의 중심이라 할 수 있는 램지 이론입니다.

### 램지 이론

'램지 이론'이라고 하면 가장 먼저 떠오르면서 실제로도 제일 중요한 것이 학부 이산수학 과목에서도 접할 수 있는 '램지 수' 라 할 수 있습니다. $N$명의 사람들이 있으면 항상 서로 친구관계인 $k$명이 있거나 서로 친구관계가 아닌 $t$명의 사람이 있을 최소의 $N$ 값을 램지 수 $R(k,t)$라 합니다. 대표적인 예로 6명의 사람이 있으면, 이 중에서는 항상 서로 모두 페이스북 친구인 3명이 있거나 서로 모두 친구가 아닌 3명이 있게 되지만, 5명의 경우 이런 사실이 성립하지 않을 수도 있습니다. 따라서 $R(3,3)=6$인 것이죠. 이러한 수가 항상 존재한다는 정리가 바로 [램지 정리](https://ko.wikipedia.org/wiki/램지의_정리)입니다.

아직도 $R(6,6)$의 정확한 값도 모를 정도로 램지 수를 완전하게 계산해 내는 데에는 한계가 많기 때문에 지금까지의 연구는 주로 $R(3,t), R(4,t),\cdots$와 같이 두 변수 중 하나의 값을 고정시키거나, $R(k,k)$와 같이 $k=t$인 경우에 주목해 왔습니다. 특히 $\lim_{k\rightarrow\infty}R(k,k)^{1/k}$이 존재하는가 라는 문제는 20세기의 전설적인 수학자 에르되시(Erdős)가 100달러를 상금으로 걸어놓은 조합론의 가장 중요한 미해결 난제 중 하나입니다.

현재까지 전자의 $R(3,t)$ 케이스가 현재 상계와 하계가 4배밖에 차이가 나지 않을 정도로 연구가 진척된 반면(여기에 대해서는 다음에 더 자세히 다뤄 보도록 하겠습니다) 후자, 즉 대각 램지 수(diagonal Ramsey Number)라 불리는 $R(t,t)$의 경우 연구 결과가 많지 않았습니다. 에르되시(Erdős)와 세케레시(Szekeres)가 1935년 처음으로 $R(k,k)\leq \binom{2k-2}{k-1}$임을 보였고, 그 뒤 반세기가 더 지난 87년에서야 이번 2014년 ICM 기조강연자이기도 한 [Vojtěch Rödl](https://www.math.emory.edu/~rodl/) 교수가

$$\lim_{k\rightarrow\infty}\frac{R(k,k)}{\binom{2k-2}{k-1}}=0$$

임을 보였습니다 (이 결과들은 사실 $R(k,t)$의 경우에 대해서도 일반화가 가능합니다.) 그리고 같은 해 [Thomason](https://www.maths.cam.ac.uk/person/agt2) 교수가 이 상계를 개선해서 어떤 양의 상수 $A$에 대해

$$R(k,k)\leq k^{-1/2+A/\sqrt{\log k}}\binom{2k-2}{k-1}$$

임을 증명했습니다. 그리고 다시 20여년이 지나서야 콘론 교수가

$$R(k,k)\leq k^{-C\frac{\log k}{\log\log k}}\binom{2k-2}{k-1}$$

라는 결과를 얻었고, 지금까지 이 상계가 최선의 결과입니다. 이 결과는 처음으로 아무리 큰 상수 $A$를 가지고 와도 점근적으로 $R(k,k)<k^{-A}\binom{2k-2}{k-1}$임을 보인 것으로, 수학 분야의 최고 학술지라 할 수 있는 Annals of Mathematics에 실렸습니다. ([논문링크](https://annals.math.princeton.edu/2009/170-2/p15)) 참고로 하계의 경우 [Spencer](https://cs.nyu.edu/~spencer/)의 1975년 결과가 아직도 깨지지 않고 있고, 상계와 그 간극이 작지 않습니다.

### 옮김 정리

콘론 교수의 최근 연구 중 주목받는 것은 Gowers 교수와 함께 한 옮김 정리(Transference Principle)에 관한 연구입니다. 이 결과는 '소수 안에는 모든 (유한한) 길이의 등차수열이 있다'는 [그린-타오 정리](https://ko.wikipedia.org/wiki/그린-타오_정리)의 그래프 버전이라고 할 수 있습니다.

그린-타오 정리의 핵심이 되는 부분은 '자연수 안에서 양의 밀도를 갖는 수열 안에는 모든 유한한 길이의 등차수열이 있다'는 Szemerédi의 정리의 가정을 소수로 '옮겨(transfer)' 오는 것인데, 그린-타오 정리가 처음 증명된 이후 Gowers, 그리고 Reingold-Trevisan-Tulsiani-Vadhan 그룹 등에 의해 이 부분의 더 단순한 증명을 찾는 연구가 계속되었습니다. Conlon 교수와 Gowers 교수는 이 옮김 정리의 그래프 이론 버전을 개발해서 랜덤 그래프 이론의 여러 가지 문제들을 한꺼번에 해결하는 결과를 얻었습니다. 비슷한 결과가 [Schacht](https://www.math.uni-hamburg.de/home/schacht/)에 의해서도 독립적으로 증명되었고, 후속 연구를 했던 [Samotij](https://www.dpmms.cam.ac.uk/~ws299/)까지 네 명의 연구자가 모두 함께 또 하나의 논문을 내기도 했습니다. 이 증명은 함수해석학의 [한-바나흐 정리](https://ko.wikipedia.org/wiki/한-바나흐_정리)를 기반으로 하고 있어 놀랍기도 하거니와, 해석학이 조합론에 얼마나 광범위하게 쓰일 수 있는지를 보여 주는 하나의 예가 되었습니다.

또한 콘론 교수는 이 경험을 바탕으로 최근 [Fox](https://stanford.edu/~jacobfox/), [Zhao](https://yufeizhao.com) 와 함께 그린-타오 정리의 증명을 간단히 하는 연구를 계속 진행했고, 그 결과 원래 60페이지가 넘던 증명을 25페이지까지 줄이기도 했습니다.

콘론 교수는 앞으로도 여러 가지 램지 이론, 조합적 정수론, 랜덤 그래프 이론을 연결시키는 극단 조합론의 여러가지 문제들을 연구할 계획입니다. 콘론 교수가 이번 ICM에서 어떤 내용의 발표를 할지는 [https://www.its.caltech.edu/~dconlon/ICMPaper.pdf](https://www.its.caltech.edu/~dconlon/ICMPaper.pdf) 에서 미리 확인할 수 있는데, 지금까지 연구 결과를 잘 정리함과 동시에 앞으로 이 분야의 연구가 나아갈 방향도 제시하는 좋은 논문입니다. 관련 분야에 전문적인 관심이 있는 독자들에게 일독을 권합니다.