# 캡스톤 주제 조사
> 캡스톤 주제 선정을 위해 각 팀원 자료 조사 내용 정리

### 1. KakaoTalk DB 암호화 루틴 분석 및 복호화
로컬에 저장되는 톡내용을 복호화 하는 과정. 리버싱 어려워 보이는데, 최근 사례도 상세하고 목표도 확실함. 

* **결과물:** DB 복호화 도구 / 분석 보고서
* **기타 메모:**
  * 현재 최신 버전의 카카오톡과 25년도와의 비교 확장 가능 (차별성)
  * 과거에는 UserId (실제 카톡 가입 시 부여받는 개인식별 번호)가 쉽게 노출됐다고 함 (지금은 아닌듯)
  * mac의 경우, UserId와 하드웨어 UUID로 암/복호화 키를 생성한다고 함
  * 암호화 모듈이 추가된 SQLite 사용
  * IDA Pro로 동적 분석, HxD로 파일 시그니처 확인 했다고함
  * 환경(윈도우, 맥, 안드로이드) 선택 필요. 안드로이드의 경우 연구는 없지만, 도구는 존재한다고 함
* **참고 링크:**
  * [25년도 분석 자료 - 이거 젤 중요](https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART003256893)
  * [macOS 분석 자료](https://public.thinkonweb.com/journals/jkiisc/digital-library/56149)
  * [안드로이드 복호화 툴](https://github.com/jiru/kakaodecrypt)

---
