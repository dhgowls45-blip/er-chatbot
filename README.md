# 응급실 챗봇 - 배포 가이드

## 📁 파일 구성
```
chatbot-pwa/
├── index.html       ← 메인 챗봇
├── manifest.json    ← PWA 앱 정보
├── sw.js            ← 오프라인 지원
├── netlify.toml     ← Netlify 설정
├── icons/
│   ├── icon-192.png
│   └── icon-512.png
└── README.md
```

---

## 🚀 Netlify 배포 방법 (무료, 5분)

1. **https://netlify.com** 접속 → 무료 회원가입
2. 대시보드에서 **"Add new site" → "Deploy manually"** 클릭
3. **이 폴더 전체를 드래그 앤 드롭**
4. 배포 완료! 자동으로 주소가 생성됩니다 (예: `er-chatbot-abc123.netlify.app`)

---

## 📱 핸드폰에 앱으로 설치하기

### Android (크롬)
- 배포된 주소 접속 → 상단에 "설치" 배너 팝업 → **설치** 탭

### iPhone (Safari)
1. Safari로 주소 접속
2. 하단 공유 버튼(□↑) 탭
3. **"홈 화면에 추가"** 선택
4. 추가 → 홈 화면에 🏥 아이콘 생성

---

## ✏️ FAQ 내용 수정하기
`index.html` 파일을 열고 아래 부분을 수정:
```js
const noticeDate = "2026-05-14";       // ← 날짜
const noticeContent = "공지 내용...";  // ← 공지
```

FAQ 데이터는 **FAQ 관리 탭**에서 직접 추가/삭제 가능합니다.
(입력한 내용은 핸드폰 로컬에 자동 저장됩니다.)

---

## 📌 주소 공유
배포 후 생성된 Netlify 주소를 팀원들에게 카카오톡 등으로 공유하면
누구나 앱처럼 설치해서 사용할 수 있습니다.
