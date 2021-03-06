---
casestudy:
    title: '관계형 스토리지 솔루션 디자인'
    module: '관계형 스토리지 솔루션'
---
# 관계형 스토리지 디자인 사례 연구

소요 시간: 90분

## 요구 사항

Tailwind Traders는 기존 공용 웹 사이트 데이터베이스를 Azure로 이동하려고 합니다. 웹 사이트 프런트 엔드도 Azure로 이동할 예정이기 때문입니다.  처음에는 중복성 보장을 위해 2개 지역에만 웹 사이트 프런트 엔드를 배포할 계획입니다.  하지만 트래픽이 늘어나면 전 세계의 여러 지역으로 웹 사이트를 복제할 예정입니다. 여러분이 마이그레이션 요청을 받은 데이터베이스에는 제품 카탈로그와 모든 온라인 주문 정보가 저장되어 있습니다.  이 데이터베이스는 현재 온-프레미스의 Microsoft SQL Server Always On 가용성 그룹 하나에서 실행됩니다.

Tailwind Traders가 중요하게 고려하는 주요 사안은 다음과 같습니다.

-	**고가용성.**  이 데이터베이스는 업무상 반드시 필요하므로, Tailwind Traders는 이 데이터베이스의 고가용성을 유지하고자 합니다.  데이터베이스 사용이 중단되면 영업 기회가 손실되거나 고객의 신뢰도가 낮아질 수 있습니다.

-	**웹 사이트 성능.**  웹 사이트의 주문 진행 성능은 좋은 편이지만, 여러 항목이 나열되어 있는 페이지를 찾아보거나 검색하는 속도가 느린 것으로 보고되고 있습니다.

-	**보안.**  Tailwind Traders는 데이터베이스에 저장된 개인 정보나 재무 정보의 노출을 철저하게 방지하려 합니다.  따라서 보안 팀은 적절한 보안 조치를 구현해야 할 뿐 아니라 가능한 경우 업계 표준 모범 사례가 구현되는지도 확인해야 합니다.


## 작업

1.	데이터베이스 솔루션을 디자인하세요. 디자인 과정에서는 권한 부여, 인증, 가격 책정, 성능 및 고가용성을 고려해야 합니다. 
2.	최종적으로 결정한 솔루션을 다이어그램으로 그려서 설명하세요. 

안정적이며 효율적인 고품질 클라우드 아키텍처를 생성하려면 Well-Architected Framework 원칙을 어떻게 통합해야 하나요?
