💡 Prompt Engineering & Retrieval 기반 QA 시스템 요약
🧠 핵심 개념 요약
🔁 Latency & Bandwidth 개념
Latency: 첫 토큰이 나올 때까지의 시간 (응답 지연 시간)

Bandwidth: 전체 응답의 처리 속도

연산량과 대역폭 고려는 LLM 최적화에 중요!

🛠️ 프롬프트 엔지니어링 (Prompt Engineering)
프롬프트 엔지니어링의 핵심은 컨텍스트를 명확하게 제공하는 것입니다.

✅ 핵심 전략 (OpenAI 권장)
명확한 지시 작성 (Write clear instructions)

참고 텍스트 제공 (Provide reference text)

복잡한 작업은 분해 (Split complex tasks)

모델에게 ‘생각할 시간’ 주기 (Give time to think)

외부 도구 활용 (Use external tools)

변경 사항을 체계적으로 테스트 (Test changes systematically)

주의: 어설픈 지시/설명은 오히려 성능 저하 → 프롬프트는 간결하게 써야 함

🧪 반복과 피드백 (Iteration)
공식 튜토리얼 숙지 후,

내 문제를 명료하게 구조화

→ 지시 → 피드백 → 반복(iteration)은 필수

📚 참고 자료 (믿을 수 있는 공식 자료만)
OpenAI Official guide https://platform.openai.com/docs/guides/prompt-engineering/
Best practices https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-the-openai-api
Microsoft guide https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/advanced-prompt-engineering?pivots=programming-language-chat-completions


⚠️ 유튜브에 떠도는 비공식 가이드는 신뢰성 떨어질 수 있음. 위 링크만 참고할 것!

🧩 Prompt 버전 관리 도구
도구	설명
AWS Prompt Management	AWS 기반 프롬프트 관리
Langchain Prompt Hub	LangChain에서 프롬프트 버전 관리
Langfuse	프롬프트 및 실험 관리 도구
PromptHub	평가 기반 버전 관리 및 메트릭 관리 가능

📖 Retrieval 기반 QA 시스템의 핵심 용어 정리
카테고리	역할	예시 설명
Query Construction	쿼리를 어떻게 만들까	사용자 질문을 SQL/벡터 질의로 변환
Query Translation	쿼리를 더 잘 검색되게 바꿈	질문을 재작성/분해 (예: RAG-Fusion)
Routing	어디서 검색할지 결정	벡터 DB vs 그래프 DB 선택, 프롬프트 고르기
Retrieval	문서를 찾는 과정	검색 → 랭킹 → 필터링 → 결과 추출
Indexing	문서를 검색 가능하게 준비	문서 분할, 임베딩, 인덱스 트리 구축
Generation	LLM이 최종 답변 생성	문서를 바탕으로 GPT가 응답 생성

꼭 알아야 할 기술: Attention, Embedding, Vector Search, RAG (Retrieval-Augmented Generation)

