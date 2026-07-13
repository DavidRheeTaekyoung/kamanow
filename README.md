# KAMANOW — KAMA 【K-POP American Music Awards】 Official Fan Platform (MVP)

KBS × U.S. Media Group 주최 K-POP 글로벌 음악 시상식 **KAMA**의 공식 팬 플랫폼 홈페이지 MVP.

- 개최: 2027년 4월 3일 · SoFi Stadium, Los Angeles
- 슬로건: "Fans Vote. Fans Influence. Fans Celebrate."

## MVP 포함 기능 (전부 클릭 동작, 결제 모듈 미연동)

| 기능 | 상태 |
|---|---|
| 팬 투표 (Round 1/2/3 · Regional) | ✅ 데모 동작 (Rewards 차감·순위 반영) |
| 실시간 랭킹 (Global/대륙별/팬덤) | ✅ 탭 전환 동작 |
| 아티스트 페이지 | ✅ 카드 그리드 (상세는 본 개발) |
| 티켓 예매 (4개 등급) | ✅ 수량 선택 → 체크아웃 데모 |
| 굿즈 스토어 + 장바구니 | ✅ 담기·합계·체크아웃 데모 |
| 멤버십 ($4.99/$9.99) + Rewards 충전 | ✅ 데모 동작 |
| 광고 시청 리워드 (+10 Rewards) | ✅ 데모 동작 |
| 로그인/국가 인증(대륙 자동 구분) | ✅ UI만 (인증·Anti-Voting은 본 개발) |
| 결제 (카드·Apple/Google Pay·PayPal 등) | ⏳ 추후 모듈 연동 |

## 배포 (GitHub Pages)

```bash
git clone https://github.com/DavidRheeTaekyoung/kamanow.git
cd kamanow
# 이 폴더의 index.html, README.md 복사 후
git add . && git commit -m "KAMA fan platform MVP" && git push origin main
```

GitHub 저장소 → Settings → Pages → Branch: `main`, 폴더 `/` 선택 → 저장.
수 분 후 `https://davidrheetaekyoung.github.io/kamanow/` 에서 접속 가능.

## 구조

- `index.html` — 단일 파일 (HTML/CSS/JS 통합, 외부 의존성은 Google Fonts뿐)
- 아티스트/투표 수치는 데모 데이터. `index.html` 내 `artists`, `goods` 배열만 교체하면 됨.
