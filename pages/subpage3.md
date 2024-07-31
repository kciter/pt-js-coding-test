---
title: 문제 유형 파악하기
layout: section
subject: 문제 유형 파악하기
---

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 문제 접근 전략

* 문제 유형을 바로 파악하는 것보다 <accent>가능성을 좁혀나가는 것</accent>이 중요
* 문제에서 유형을 좁힐 수 있는 힌트는?
  * 입출력 제한
  * 문제 키워드
  * 이미지
  * 문제 순서
* 문제를 잘 읽는 것이 중요

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 입출력 제한을 먼저 확인하자

* 문제를 읽기 전에 입출력 제한부터 확인해보자
* 다음과 같이 분류해볼 수 있다
  * 입력이 100 이하인 경우 (N <= 100)
    * 완전 탐색
    * 백트래킹
    * 시뮬레이션
    * <accent>구현 문제</accent>
  * 입력이 10,000 이하인 경우 (N <= 10,000)
    * 최대 O(n^2) 이내로 풀어야하는 문제
    * 혹은 n이 100 이하일 때 이중 반복문으로 풀 수 있는 문제

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 입출력 제한을 먼저 확인하자

* 문제를 읽기 전에 입출력 제한부터 확인해보자
* 다음과 같이 분류해볼 수 있다
  * 입력이 1,000,000 이하인 경우 (N <= 1,000,000)
    * 최대 O(n log n) 이내로 풀어야하는 문제
    * 힙, 우선순위 큐
    * 정렬
    * 동적 계획법
    * 위상정렬
    * 다익스트라 알고리즘
  * 입력이 100,000,000 이하인 경우 (N <= 100,000,000)
    * 최대 O(n) 이내로 풀어야하는 문제
    * 동적 계획법
    * 그리디

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 입출력 제한을 먼저 확인하자

* 문제를 읽기 전에 입출력 제한부터 확인해보자
* 다음과 같이 분류해볼 수 있다
  * 입력이 100,000,000 보다 큰 경우 (N > 100,000,000)
    * 최대 O(log n) 이내로 풀어야하는 문제
    * 거의 안나오는 유형이거나 입력 제한 자체가 함정인 경우
    * 이진 탐색

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 입출력 제한을 먼저 확인하자

* 문제를 읽기 전에 입출력 제한부터 확인해보자
* 다음과 같이 분류해볼 수 있다
  * 입력이 100,000,000 보다 큰 경우 (N > 100,000,000)
    * 최대 O(log n) 이내로 풀어야하는 문제
    * 거의 안나오는 유형이거나 입력 제한 자체가 함정인 경우
    * 이진 탐색

---
layout: center
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

<Image src="/heap-problem.png" width="540px" />

입력 제한을 보고 판단해보자!

---
layout: center
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

<Image src="/simulation-problem.png" width="540px" />

입력 제한을 보고 판단해보자!

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 키워드로 유형 좁히기

* X라는 조건을 만족하는 가장 최대/최소값을 찾아라
  * 높은 확률로 이진 탐색(파라메트릭 서치)를 통해 푸는 것이 가능

- - -

<Image src="/keyword-1.png" width="540px" />

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 키워드로 유형 좁히기

* 계속해서 최소 혹은 최대값을 알야하는 경우
  * 높은 확률로 힙을 사용해야 하는 문제

- - -

<Image src="/keyword-2.png" width="540px" />

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 이미지로 유형 좁히기

* 어떤 영역을 채워야 하는 경우
  * 높은 확률로 BFS, DFS를 이용하는 문제

- - -

<Image src="/keyword-3.png" width="540px" />

---
layout: two-cols
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

::left::
# 이미지로 유형 좁히기

* 그래프가 주어지는 경우
  * 당연히 그래프 문제일 가능성이 높음
  * 알고리즘으로 좁히면 셋 중 하나일 가능성이 높음
    * 최단 거리 찾기
    * 최소 신장 트리
    * 위상 정렬
  * 키워드도 같이 확인하자

::right::

<spacer gap="40" />

<Image src="/keyword-4.png" width="440px" />

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 유형을 한 눈에 파악하기 힘든 경우...

* 유형 파악이 익숙해져도 파악하기 어렵다면 방법론 문제일 가능성이 높다
  * 동적 계획법
    * 규칙을 찾을 수 있다면 이 유형일 가능성이 높음
  * 백트래킹
    * 아무리 생각해도 모든 경우의 수를 봐야할 것 같은 경우
    * 그렇지만 정말 모두 찾으면 시간 초과가 날 것 같은 경우
  * 그리디
    * 직관적으로 풀어낼 수 있다면 이 유형일 가능성이 높음

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 문제 순서로 좁히기

* 보통 뒤로 갈수록 난이도가 올라가는 경우가 많음
* 문제 순서를 보고 유형을 파악해보자
  * 처음 문제는 구현 문제일 가능성이 높음
    * 문자열 처리, 시뮬레이션 등
  * 중간 문제는 유형 문제일 가능성이 높음
    * 힙, BFS, 트리, 그래프 등
  * 마지막 문제는 방법론 유형일 가능성이 높음
    * 동적 계획법, 백트래킹, 그리디 등
* 첫 문제부터 동적 계획법을 요구하는 문제가 나오는 경우는 거의 없다

---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 문제를 잘 읽기

* 수능 언어 지문처럼 보자
* 문제 읽다가 시간 다 간다!
  * 입출력 먼저 읽고
  * 훑으면서 중요 키워드 탐색
  * 예외사항이 있는지 확인


---
layout: default
headerEnable: true
headerTitle: 코딩테스트 대비 취업 특강
---

# 엣지 케이스에 대하여

* 보통 엣지 케이스는 입출력과 큰 관련이 있다!
  * 일부러 문제에서 만든 엣지 케이스는 입력이 특이한 경우가 많음
  * 입력 값의 크기가 굉장히 작은 케이스 (대부분의 입력 값이 최대값 언저리인 경우)
  * 입력 값의 크기가 굉장히 큰 케이스 (대부분의 입력 값이 최소값 언저리인 경우)
  * 입력 값의 범위가 넒은 케이스 (A는 최소값이고 B가 최대값인 경우)
  * 음수 입력이 허용된 경우 음수만 입력받는 케이스
  * 리스트를 입력 받을 때 값이 없거나 하나만 있는 케이스
* 혹은 문제를 잘 보면 알 수 있는 예외 사항
* 나머지는 내가 그냥 놓친 것

