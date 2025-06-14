# 🙌 장소 추가 기여 방법 (CONTRIBUTING)

감사합니다! 이 프로젝트는 작업하기 좋은 장소를 함께 만들어가는 오픈소스 프로젝트입니다.

## ✅ 기여 조건

아래 조건을 충족하는 장소만 등록해 주세요:

- 📶 와이파이가 안정적으로 연결될 것
- 🔌 콘센트가 충분히 있을 것
- 💺 조용한 분위기 (시끄러운 브런치 카페 등 제외)
- ❌ 프랜차이즈는 기준 미달 시 제외될 수 있음
- ❌ 시끄러운 브런치 카페, 자리 회전율 높은 테이블 매장은 제외 권장

## 📝 추가 방법

1. 이 레포를 `Fork` 합니다
2. `data/지역이름.json` 파일을 엽니다  
   (예: `data/seoul.json`, 없으면 새로 만드셔도 됩니다)
3. 아래 양식에 따라 JSON 데이터를 추가합니다:

```json
{
  "name": "카페 시그널 강남",
  "description": "커피 맛이 좋고, 좌석이 넉넉하며, 조용한 분위기.",
  "address": "서울 강남구 테헤란로 123",
  "lat": 37.123456,
  "lng": 127.123456,
  "wifi": "빠름",
  "power": "보통",
  "seat_count": "보통",
  "open_hours": "09:00 - 22:00",
  "url": "https://example.com",
  "restroom": "실내/남녀 공용",
  "images": []
}
```

> 필수 항목: `name`, `address`, `lat`, `lng`, `wifi`, `power`, `seat_count`, `open_hours`, `url`, `restroom`

4. PR(Pull Request)을 보내주세요!

## 📄 PR 제목 예시

- `서울/카페 시그널 강남 추가`
- `부산/카페 라떼리 수정`

## 🧪 유효성 검사

모든 PR은 schema/place.schema.json 기준으로 자동 검증됩니다.
JSON이 잘못되면 PR이 merge되지 않을 수 있으니 https://jsonlint.com 등으로 미리 확인해 주세요.

---

감사합니다! 🙏
기여자 목록에 자동으로 포함되며, https://place.until.blog 서비스에 실시간 반영됩니다.
