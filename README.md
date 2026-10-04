# 이병철 (LEEbyeongchul)

경희대학교 빅데이터응용학과 · 데이터/ML 엔지니어링

데이터분석과 ml,Ai엔지니어링에 관심이 있습니다.



---

## 프로젝트

| 프로젝트 | 무엇을 했나 | 스택 |
| :-- | :-- | :-- |
| **[온톨로지 금융 QA 에이전트](https://github.com/LEEbyeongchul/ontology-financial-qa-agent)**<br><sub>미래에셋증권 AI Festival 2026 · 3인</sub> | 금융 질문을 SQL로 옮겨 **근거와 함께** 답하는 에이전트. "이 데이터에 없는 축"을 선언으로 막아 그럴듯한 오답을 차단. 평가 2주간 서버 상시 가동 | HyperCLOVA X · FastAPI · SQLite · Docker |
| **[비디오 프레임 순서 복원](https://github.com/LEEbyeongchul/snu-video-frame-ordering)**<br><sub>SNU AI Challenge 2026 · 3인</sub> | VLM QLoRA 파인튜닝으로 이미지 4장의 시간 순서 복원. 지표 재정의 → 약점 구간 타깃 증강 → 우도 기반 순열 TTA (**holdout +4.76%p**) | Qwen3-VL · PEFT · PyTorch |
| **[소비기한 OCR 파이프라인](https://github.com/LEEbyeongchul/itda3-CODE-subway)**<br><sub>제3회 ITDA 연합학술제 본선 · 5인</sub> | 상품 뒷면 사진에서 소비기한 추출. 4코어 CPU·오프라인 제약 아래 경량 OCR + 날짜 해석 규칙 + 못 읽은 사진에만 재시도. 오답을 "정답이 사라진 단계"로 진단해 **봉인 500장 86.2%**(예선 84.2%), 장당 2.7~4.0초. 중고거래 식품 게시글 소비기한 자동 입력으로 기획 | PaddleOCR · OpenCV · Python |
| **[대학생 혜택 통합 서비스](https://github.com/LEEbyeongchul/2026-khuniv-NIC)**<br><sub>경희대 Nexus Innovation Challenge · 4인 · **우수상(3위)**</sub> | 결제 할인 지도와 장학금 매칭 챗봇을 한 앱으로. 크롤러 · RAG · 상태머신 챗봇 · 프론트까지 풀스택 | FastAPI · React/TS · pgvector |
| **[무임승차 수요 예측](https://github.com/LEEbyeongchul/Seoul-Subway-FreeRide-Analysis)**<br><sub>머신러닝 수업 팀 프로젝트</sub> | 지하철 노인 무임승차 2050년 수요 전망과 요금 정책 시뮬레이션. 총량 대신 **1인당 승차율 × 인구 추계**로 타깃을 바꿔 외삽 문제를 해결, 2025년 홀드아웃 **MAPE 4.19%**·연간 총량 오차 +0.59% | XGBoost · LightGBM |

---

## 수상

- 2026.09 경희대학교 서울캠퍼스 AI·SW 융합 페스티벌 **대상(1위)**
- 2026.08 경희대학교 Nexus Innovation Challenge **우수상(3위)** · 대학생 혜택 통합 서비스

---

## 작업 방식

**측정 도구를 먼저 검증합니다.** SNU 과제에서는 후보 모델 5개가 전부 무작위 수준인데 정확도가 7~16%로 나오는 모순을 발견했습니다. 원인은 항등 순서 편향이었고, 지표를 다시 정의한 뒤에야 실험이 의미를 갖기 시작했습니다.

**안 되는 것도 기록합니다.** CoT SFT −4.4%p, hard shuffle −1.1%p처럼 기각한 접근을 수치와 원인까지 남깁니다. 다음 사람이 같은 길을 다시 걷지 않도록.

**끝난 뒤에 다시 봅니다.** 금융 에이전트의 가드를 규칙 목록으로 짰는데, 대회가 끝나고 던져본 질문에서 목록에 없던 컬럼으로 또 틀렸습니다. 목록이 아니라 성질로 판정했어야 했다는 걸 그때 알았습니다.

---

## 다루는 것

`Python` `PyTorch` `Transformers / PEFT` `scikit-learn` `XGBoost · LightGBM`
`FastAPI` `SQLite · PostgreSQL` `Docker` `React · TypeScript` `Pandas · NumPy`
