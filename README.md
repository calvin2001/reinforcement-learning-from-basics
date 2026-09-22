# Reinforcement Learning from Basics

『**바닥부터 배우는 강화 학습**』(노승은, 영진닷컴)을 읽고 챕터별로 정리한 학습 기록입니다.

수식을 그대로 옮겨 적는 대신, **각 챕터가 직전 챕터의 어떤 한계를 푸는지**를 중심으로 정리합니다. MDP를 알 때 → 모를 때 → 상태가 너무 많을 때로 이어지는 흐름이 이 책의 뼈대이고, 그 연결이 보이도록 쓰는 것이 목표입니다.

---

## Progress

| # | Chapter | Keywords | Note | Code |
|:--:|:--|:--|:--:|:--:|
| 01 | 강화 학습이란 | `Agent` `Environment` `Reward` | ⬜ | — |
| 02 | 마르코프 결정 프로세스 | `MP` `MRP` `MDP` | ⬜ | — |
| 03 | 벨만 방정식 | `Bellman Expectation` `Bellman Optimality` | ⬜ | — |
| 04 | MDP를 알 때의 플래닝 | `Policy Iteration` `Value Iteration` | ⬜ | ⬜ |
| 05 | MDP를 모를 때 밸류 평가 | `Monte Carlo` `TD` | ⬜ | ⬜ |
| 06 | MDP를 모를 때 최고의 정책 찾기 | `MC Control` `SARSA` `Q-learning` | ⬜ | ⬜ |
| 07 | Deep RL 첫걸음 | `Function Approximation` `PyTorch` | ⬜ | ⬜ |
| 08 | 가치 기반 에이전트 | `DQN` `Replay Buffer` `Target Network` | ⬜ | ⬜ |
| 09 | 정책 기반 에이전트 | `REINFORCE` `Actor-Critic` | ⬜ | ⬜ |
| 10 | 알파고와 MCTS | `MCTS` `AlphaGo Zero` | ⬜ | — |
| 11 | 블레이드 & 소울 비무 AI | `Applied RL` | ⬜ | — |

완료한 챕터는 `⬜`를 노트 링크로 바꿉니다 — 예: `[Note](notes/ch05.md)`

---

## 노트 형식

각 노트는 네 가지를 담습니다. 요약만 하면 책을 덮는 순간 남는 게 없어서, 세 번째와 네 번째를 반드시 채우는 것을 규칙으로 둡니다.

1. **한 줄 요약** — 이 챕터가 해결하는 문제
2. **왜 필요한가** — 앞 챕터의 어떤 한계에서 출발했는지
3. **직접 설명해보기** — 핵심 개념을 책을 덮고 내 말로 다시 쓰기
4. **막혔던 지점** — 이해가 안 됐던 부분과, 어떻게 풀었는지

---

## 구조

```
notes/    챕터별 정리 (ch01.md ~ ch11.md)
code/     직접 구현한 코드 (ch04 ~ ch09)
```

---

## 실행 환경

```bash
pip install torch numpy matplotlib gymnasium
```

책의 예제는 `gym` 기준이며, 현재는 후속 패키지인 `gymnasium`을 사용합니다. `env.step()`의 반환값 개수가 달라져 있어 예제 코드를 그대로 돌리면 동작하지 않습니다.

---

## References

- 책 공식 코드 저장소 — [seungeunrho/RLfrombasics](https://github.com/seungeunrho/RLfrombasics)
- 저자 유튜브 채널 — 팡요랩

> 이 저장소에는 책 본문이나 그림을 옮기지 않습니다. 모든 정리는 직접 쓴 글이며, 코드 역시 직접 구현한 것입니다.
