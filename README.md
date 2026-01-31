# 🐾 PetCare AI - 반려동물 건강 관리 PWA

<div align="center">
  <img src="icon-512.png" alt="PetCare Logo" width="200"/>
  
  **반려동물의 건강, 식단, 예방접종, 병원 기록을 한 곳에서 관리하세요**

  [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
  [![PWA](https://img.shields.io/badge/PWA-Ready-green.svg)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps)
</div>

---

## ✨ 주요 기능

### 🐶 반려동물 관리
- 반려동물 프로필 등록 (이름, 종류, 품종, 생년월일, 체중)
- 사진으로 추억 기록
- 여러 반려동물 관리 (무료: 3마리, Pro: 무제한)

### 💉 건강 기록
- **예방접종 기록** - 접종 날짜, 종류, 다음 접종일 자동 알림
- **투약 일정** - 약 이름, 복용 주기 관리
- **병원 방문 기록** - 병원명, 진료 내용, 의료비 추적

### 🍖 식단 관리
- 급여 기록 (종류, 제품명, 급여량, 칼로리)
- 일일 통계 (급여 횟수, 총 칼로리)
- 반려동물별 식단 필터링

### 📊 통계 & 인사이트
- 체중 변화 그래프
- 월간 의료비 차트
- AI 기반 건강 인사이트
- 활동 요약 (최근 3개월/1년)

### 🏥 병원 찾기
- 내 위치 기반 근처 동물병원 검색
- 지역별 검색
- 전화 연결, 지도 보기

### 👨‍👩‍👧‍👦 가족 공유
- 가족 구성원 초대
- 함께 반려동물 기록 관리
- 권한 설정 (관리자/구성원)

### 📱 PWA 기능
- 홈 화면 추가 가능
- 오프라인 지원
- 푸시 알림 (예방접종, 투약 알림)

---

## 🚀 기술 스택

### Frontend
- **HTML5** - 시맨틱 마크업
- **CSS3** - 다크 테마, 그라데이션, 애니메이션
- **JavaScript (ES6+)** - Vanilla JS, 모듈 패턴
- **Chart.js** - 데이터 시각화

### PWA
- **Service Worker** - 오프라인 캐싱
- **Web App Manifest** - 설치 가능한 앱
- **Notification API** - 푸시 알림

### Storage
- **localStorage** - 로컬 데이터 저장 (5MB)
- **IndexedDB** - 대용량 이미지 저장

### APIs
- **Geolocation API** - 위치 기반 병원 검색
- **Web Share API** - 사진 공유
- **FileReader API** - 이미지 업로드
- **Canvas API** - 이미지 압축

---

## 📦 설치 및 실행

### 웹사이트 접속
```
https://your-netlify-url.netlify.app
```

### 로컬 개발
```bash
# 저장소 클론
git clone https://github.com/YOUR_USERNAME/petcare-app.git
cd petcare-app

# 로컬 서버 실행 (Python)
python -m http.server 8000

# 또는 (Node.js)
npx serve

# 브라우저에서 열기
http://localhost:8000
```

### PWA 설치
1. Chrome/Edge/Safari에서 웹사이트 접속
2. 주소창 오른쪽 "설치" 버튼 클릭
3. 홈 화면에 추가됨!

---

## 🎯 프리미엄 기능

### 무료 (Free)
- ✅ 반려동물 3마리
- ✅ 사진 10장
- ✅ 가족 2명
- ✅ 기본 통계

### Pro (₩4,900/월 또는 ₩49,000/년)
- ✅ 무제한 반려동물
- ✅ 무제한 사진
- ✅ 무제한 가족 구성원
- ✅ 광고 제거
- ✅ 클라우드 백업
- ✅ 우선 고객 지원

---

## 📱 지원 브라우저

| Browser | Desktop | Mobile |
|---------|---------|--------|
| Chrome  | ✅      | ✅     |
| Safari  | ✅      | ✅     |
| Edge    | ✅      | ✅     |
| Firefox | ✅      | ✅     |
| Samsung Internet | - | ✅ |

---

## 🛠️ 개발 로드맵

### Phase 1 ✅ (완료)
- [x] 기본 CRUD 기능
- [x] PWA 변환
- [x] 통계 대시보드

### Phase 2 ✅ (완료)
- [x] 사진 앨범
- [x] 식단 관리
- [x] 병원 찾기

### Phase 3 ✅ (완료)
- [x] 가족 공유
- [x] 알림 시스템
- [x] 프리미엄 구독

### Phase 4 ⏳ (진행 중)
- [ ] Firebase 백엔드
- [ ] 계정 시스템 (Google/이메일 로그인)
- [ ] 클라우드 동기화
- [ ] 실제 결제 연동 (Toss Payments)

### Phase 5 🔮 (계획)
- [ ] React Native 모바일 앱
- [ ] AI 건강 분석 (Claude API)
- [ ] 수의사 상담 연결
- [ ] 커뮤니티 기능

---

## 🐛 알려진 제한사항

1. **localStorage 용량 제한** (5MB)
   - 사진 많을 경우 용량 부족 가능
   - 해결: IndexedDB 또는 클라우드 저장소 (Phase 4)

2. **기기별 데이터 저장**
   - 다른 기기에서 접근 불가
   - 해결: 데이터 내보내기/가져오기 기능 제공

3. **브라우저 알림 제한**
   - 앱이 닫혀있으면 알림 안 옴
   - 해결: FCM 푸시 알림 (Phase 4)

---

## 📄 라이선스

MIT License - 자유롭게 사용, 수정, 배포 가능합니다.

---

## 🙏 기여하기

버그 리포트, 기능 제안, Pull Request 환영합니다!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📞 문의

- **Email**: support@petcare.app (설정 필요)
- **Website**: https://petcare.app
- **Issues**: GitHub Issues

---

## 🎉 만든 사람

**Claude AI** - AI 어시스턴트와 함께 개발한 프로젝트

---

<div align="center">
  Made with ❤️ for pet lovers
  
  **⭐ 이 프로젝트가 도움이 되었다면 스타를 눌러주세요!**
</div>
