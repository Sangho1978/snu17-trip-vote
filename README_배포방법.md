# 2026 하반기 국외연수 선호도 투표 사이트 v3

## 포함 내용
- index.html: GitHub Pages용 단일 페이지 앱
- assets/images/display: 모바일 표시용 최적화 이미지
- assets/images/original: 다운로드용 원본 이미지
- assets/pdfs: 상세 PDF 파일
- firebase-rules-test-only.json: 테스트용 Firebase Realtime Database 규칙 예시

## 배포 방법
1. 이 폴더의 모든 파일과 폴더를 GitHub 저장소 루트에 업로드합니다.
2. GitHub 저장소 Settings > Pages에서 main / root 배포를 켭니다.
3. Firebase Console에서 프로젝트를 만들고 Realtime Database와 Authentication > Anonymous를 활성화합니다.
4. index.html 상단의 FIREBASE_CONFIG 값을 Firebase 웹 앱 설정값으로 교체합니다.
5. Firebase Realtime Database Rules에는 테스트 시 firebase-rules-test-only.json 내용을 적용할 수 있습니다. 운영 전에는 관리자 권한 검증 방식을 별도로 강화하는 것이 좋습니다.

## 후보지
1. 북미 동부 | 메이플 로드
2. 뉴질랜드 남섬 | 퀸스타운 + 마운트쿡
3. 크로아티아 | 아드리아해 + 두브로브니크
4. 스페인 남부 | 안달루시아
5. 아이슬란드 | 골든서클 + 남부해안
6. 남프랑스 | 지중해 + 프로방스
7. 이집트 | 나일 크루즈 + 홍해
8. 영국·프랑스 | 런던 + 파리
9. 미국 서부 | LA + 요세미티 + 샌프란시스코
10. 스페인 북부 | 100km 순례길 도보
11. 이탈리아 북부 | 베네치아 + 돌로미티 + 밀라노

## 주의
- FIREBASE_CONFIG가 비어 있으면 브라우저 로컬 테스트 모드로만 작동하며, 사용자 간 실시간 공유가 되지 않습니다.
- GitHub Pages + Firebase 방식은 정적 페이지 기반이므로, 강한 인증이 필요한 경우 Firebase Cloud Functions 또는 별도 서버 검증을 추가해야 합니다.
