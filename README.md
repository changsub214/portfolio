# portfolio
포트폴리오 마스터링크로 공개가능한 자산에 한하여 링크제공

[2026]
■ 통신사 데이터레이크 온톨로지 PoC
정형 데이터와 비정형 문서를 BigQuery에 적재하고, 현업 핵심 질문(CQ) 기반으로 두 데이터를 잇는 2계층 그래프 모델 설계. GraphRAG 에이전트와 근거 경로 시각화 구현

- 임원 브리핑, 1단계 PoC 검증 통과
- Google Cloud 내 초기 레퍼런스로 확산, 핵심 멤버 지정

■ 금융 심사 에이전트 데모
감독규정과 내규 조항의 단서, 위임, 충돌 관계를 정형 데이터와 결합해 그래프로 모델링. 문서 표준화(OKF)와 Knowledge Catalog 거버넌스 적용

- 자체 설계 문항 정확도: RAG 75% → Graph 100%
→ https://finance-ontology-studio-567090080191.us-central1.run.app/okf_veri_web/index.html

■ Apache Iceberg on GCP 검증
카탈로그 3종, Compaction, Dataproc 엔진 성능 비교 노트북 구현, 고객 및 파트너사 배포
→ https://github.com/changsub214/iceberggcp

■ 그래프·배치 파이프라인

- Spanner Graph 정형·비정형 적재 파이프라인 및 실습 구축, 고객 대상 5회+ 운영(1개사 PoC 확대)
- YouTube API→Composer 배치→BigQuery 적재→NL2SQL 에이전트 분석 환경 구축, 제조 고객 시연
- Next '26 BigQuery 신기능 7종 실행 노트북 제작·공유
→ https://github.com/changsub214/next26-krda

■ 문서 메타데이터 품질 자동화
5개 에이전트와 LLM-as-a-Judge 품질 게이트(통과/반려 재작업 루프)로 불량 메타데이터 유입 차단, Knowledge Catalog 게시
→ https://github.com/changsub214/okf_harness_for_gemini

■ 문서·그래프 통합 분석 에이전트
비정형 문서 표준화(OKF)와 정형 데이터 그래프를 결합해 환각 및 문서 토큰 과다 소모 문제 개선
→ https://github.com/changsub214/okf-bq-agent

■ 통신사 네트워크 PoC
해외 리전 모델 사용 제약에 대응해 오픈소스 LLM을 국내 리전에 배포 및 RAG 구현, Dataform과 Dataflow 파이프라인 담당

■ 교육
BigQuery 대화형 에이전트→Gemini Enterprise 구축 핸즈온 제작, 파트너사 100명+ 교육
→ https://caa-guide-web-1022535039566.us-central1.run.app/#tab-overview

[2025]
■ 금융사 MySQL→BigQuery 실시간 CDC PoC
Debezium, Kafka, Dataflow, BigQuery 파이프라인 구성 및 부하 테스트 수행

- 최대 25,403 TPS(Insert+Update 혼합 12,988 TPS), 평균 E2E 지연 0.9~1.5초
- 검증 성공 → 고객사 마이그레이션 결정

■ 증권 정형·비정형 통합 분석 데모
ML 시세 예측 모델과 Gemini로 JSON 구조화한 증권 리포트 결합. Google Cloud 행사 발표
→ https://cloudonair.withgoogle.com/events/google-cloud-onboard-h2?talk=t2-s2

■ 기타

- 멀티 데이터 에이전트 데모 → https://github.com/changsub214/kr-data-agent
- 에이전트 로그 BigQuery 적재 기반 토큰 추적 데모
- Google ADK Data Science Agent 비동기 오류 수정 PR 병합 → https://github.com/google/adk-recipes/pull/242
- 직무 워크숍 운영 체계 구축(30회+, 평균 만족도 4.5/5)
