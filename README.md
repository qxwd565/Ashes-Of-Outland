# Hearthstone Ashes of Outland API

하스스톤 **황폐한 아웃랜드 (Ashes of Outland)** 카드 데이터입니다. [Across-The-Timeways](https://github.com/qxwd565/Across-The-Timeways) 및 [legacy](https://github.com/qxwd565/legacy)와 동일한 `schema: 1` 형식을 사용합니다.

- 통합 카드 목록: [`cards.json`](cards.json)
- 원본 상세 데이터: [`source/Ashes Of Outland/`](source/Ashes%20Of%20Outland/)
- 원화 폴더: [`art/`](art/) (원화 파일은 없음)

총 **169장**, 수집 가능 **135장**, 수집 불가능 **34장**을 포함합니다.

**원화는 업로드하지 않았습니다.** 모든 카드의 `art`는 `""`이고, `art/`에는 빈 폴더 유지용 `.gitkeep`만 존재합니다.

향후 원화는 **카드 ID가 아닌 이미지 실제 바이트의 SHA-256 해시** 기반 파일명으로 관리합니다. 이미지 내용이 바뀌면 파일명이 바뀌므로 오래된 이미지 캐시와 충돌하지 않습니다. `id` 및 `dbfId`는 카드 식별과 덱 코드 연결을 위해 그대로 보존합니다.

`portrait`는 게임 내부 리소스 식별자이며 이미지 URL이 아닙니다. `nativeTags`·`relatedDbfIds`와 모든 원본 기록을 보존합니다. 통합 카드 목록은 업로드한 자료의 현재 카드 수치를 그대로 반영한 것이며, 역사적 패치 시점별 수치 재현은 별도 스냅샷에서 처리해야 합니다.
