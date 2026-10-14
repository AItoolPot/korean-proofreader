# 공개 스킬 벤치마킹 기록

조사일: 2026-10-07.
공개 저장소의 SKILL.md와 표시된 이용 조건을 비교했다.
아래 평가는 문서 검토 결과다. 다른 스킬을 실행한 성능 비교가 아니다.
링크의 main 브랜치는 이후 변경될 수 있다.

| 공개 스킬 | 참고한 설계 | 이번 스킬의 판단 |
|---|---|---|
| [DaleSeo / grammar-checker](https://github.com/DaleSeo/korean-skills/blob/main/skills/grammar-checker/SKILL.md) | 표기·문법 점검과 이유 설명을 연결한다. | 오류와 권장을 분리한다. 격식체에서 ‘10개’를 띄우도록 하는 예시는 일반 오류 규칙으로 채택하지 않는다. |
| [dotoricode / korean-humanizer](https://github.com/dotoricode/korean-humanizer/blob/main/SKILL.md) | 의미·조건·추정·말투의 보존을 구체적으로 다룬다. | 의미 보존을 핵심으로 삼는다. 단순 교정과 기술 문서를 제외하는 적용 범위는 채택하지 않는다. |
| [nyjin / korean-proofreader](https://github.com/nyjin/humanizer-ko/blob/main/skills/korean-proofreader/SKILL.md) | 문장·문단·문서를 구분하고 과잉 교정을 경계한다. | 정당한 피동과 전문어를 보존한다. 완결된 글이라는 이유로 구조 검토까지 자동 확대하지 않는다. |
| [monologg / humanizer-kr](https://github.com/monologg/humanizer-kr/blob/main/SKILL.md) | 번역투·명사 중심 표현·문체에 관한 점검 후보를 제공한다. | 실제 문맥에서 필요한 후보만 검토한다. 의견·감정 추가, 어미 혼용, AI 흔적을 지우기 위한 반복 교정은 채택하지 않는다. |

## 공식 자료와 대조한 결정

‘10개’는 숫자와 단위 명사의 붙여쓰기를 허용하는 사례다.
따라서 격식체 여부만으로 오류라고 판정하지 않는다.
근거는 [국립국어원 제43항 답변](https://www.korean.go.kr/front/onlineQna/onlineQnaView.do?mn_id=97&pageIndex=1&qna_seq=335208)이다.

보조 용언도 원칙과 허용을 구분한다.
근거는 [국립국어원 제47항 답변](https://www.korean.go.kr/front/onlineQna/onlineQnaView.do?mn_id=73&pageIndex=1&qna_seq=331002)이다.

국립국어원의 공공언어 자료에서는 호응, 어순, 번역투와 명료성을 참고했다.
공공언어의 권장 문체를 모든 글의 문법 규칙으로 적용하지 않는다.
출처와 접근 한계는 [판단 안내](language-guide.md)에 기록했다.

## 이용 조건과 작성 방식

- DaleSeo: [LICENSE](https://github.com/DaleSeo/korean-skills/blob/main/LICENSE)에서 MIT를 확인했다.
- dotoricode: [LICENSE](https://github.com/dotoricode/korean-humanizer/blob/main/LICENSE)에서 MIT를 확인했다.
- monologg: [LICENSE](https://github.com/monologg/humanizer-kr/blob/main/LICENSE)에서 MIT를 확인했다.
- nyjin: SKILL.md와 README에 MIT 표기가 있다. 별도 LICENSE 전문은 확인하지 못했다.

앞의 세 MIT 원문은 복제물이나 상당 부분을 재사용할 때 저작권·허가 고지를 포함하도록 명시한다.
이번 스킬은 외부 코드와 지침 본문을 복제하지 않았다. 설계 관점을 비교하고 지침과 예문을 새로 작성했다.
공식 자료도 본문을 묶어 재배포하지 않고 출처와 적용 판단을 정리했다.
공개 스킬의 AI 탐지 성능 수치나 연구 소개는 이번 검증의 근거로 사용하지 않았다.

## 검증 범위

검증은 새 스킬의 구조 검사와 작성자의 대표 문장 적용 검토로 한정한다.
별도 에이전트 평가, 대규모 교정 정확도 측정과 실제 자동 선택 검증은 수행하지 않았다.
