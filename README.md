# Hwei's Daily Briefing

매일 아침 8시(KST), 외식업 뉴스와 경제·트렌드 유튜브 브리핑이 자동으로 쌓이는 개인 페이지입니다.

🔗 **사이트:** https://gnlghks-harry.github.io/briefing/

## 구조
- `index.html` — 브리핑을 날짜별로 묶어 보여주는 페이지 (직접 수정 불필요)
- `news.json` — 외식업 뉴스 브리핑 데이터 (매일 자동 추가, 최신이 위)
- `youtube.json` — 경제·트렌드 유튜브 브리핑 데이터 (매일 자동 추가)

## 데이터 형식
`news.json` 각 항목:
```json
{"date":"YYYY-MM-DD","title":"...","insight":"오늘의 핵심 한 줄",
 "items":[{"title":"...","summary":"...","link":"https://..."}]}
```
`youtube.json` 각 항목: `items` 대신 `sections:[{"name":"📈 경제","items":[...]}]` 사용 가능.

> 자동 업데이트: Claude Code 아침 루틴이 매일 이 저장소에 항목을 추가(prepend)합니다.
