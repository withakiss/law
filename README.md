# 대한민국 법령 검색 웹앱

법제처 오픈 API를 활용한 간단한 법령 검색 웹 애플리케이션입니다.

## 기능

- **법령명/키워드 검색**: 법령명, 조문, 전체 검색 지원
- **필터 옵션**: 검색 유형(법령명/조문/전체), 정렬(관련도/최신/법령명), 페이지당 표시 개수
- **결과 표시**: 법령명, 종류, 공포일자, 시행일자, 소관부처 등 메타데이터 제공
- **상세 보기**: 법제처 상세 페이지로 바로 이동
- **페이지네이션**: 대량 검색 결과 페이지별 탐색
- **반응형 디자인**: 모바일/데스크톱 모두 지원

## 사용 방법

1. `index.html`을 브라우저에서 열기
2. 검색어 입력 후 검색 버튼 클릭 (엔터키도 가능)
3. 필터 옵션으로 검색 조건 조정 가능
4. 결과 카드에서 '상세 보기' 클릭 시 법제처 상세 페이지로 이동

## API 설정

법제처 오픈 API 사용을 위해 인증키(OC)가 필요합니다:

1. [법제처 오픈 API](https://www.law.go.kr/DRF/lawService.do)에서 인증키 발급
2. `index.html` 상단의 `OC` 변수에 발급받은 키 입력

```javascript
const OC = 'your-api-key-here';
```

## 파일 구조

```
openclaw_mcp_law/
├── index.html    # 메인 애플리케이션 (HTML + CSS + JS 통합)
└── README.md     # 이 파일
```

## 기술 스택

- Vanilla HTML5, CSS3, JavaScript (ES6+)
- 법제처 오픈 API (REST, JSON)
- 외부 의존성 없음 (CDN, 프레임워크 불필요)

## 브라우저 지원

- Chrome, Firefox, Safari, Edge 최신 버전
- 모바일 브라우저 지원

## 라이선스

데이터: 법제처 국가법령정보센터 오픈 API 이용약관 준수
코드: MIT License

## 참고

- [법제처 오픈 API 문서](https://www.law.go.kr/DRF/lawService.do)
- [국가법령정보센터](https://www.law.go.kr)