# 데스크 에이전트 랩

FICC S&T 영업지원 AI 에이전트를 처음 만들어보는 실습형 입문 웹사이트입니다. 챗봇을 검색 용도로만 써온 사람이 데스크 업무 하나를 골라 Claude로 실제 동작하는 에이전트를 만들어보는 5단계 커리큘럼과, 바로 따라 해볼 수 있는 목업(가상) 데이터·지시문 예시를 담고 있습니다.

- `index.html` — 사이트 전체 (빌드 도구 없이 단일 HTML 파일)
- 실습 키트(리서치 노트, 에이전트 지시문 예시)는 전부 가상의 발행사·수치로 구성되어 있어 그대로 복사해 사용해도 안전합니다. 실제 데스크 데이터로 바꿀 때는 사내 컴플라이언스 확인을 먼저 거치세요.

## Vercel로 배포하기

빌드 단계가 없는 정적 사이트라 별도 설정 없이 배포할 수 있습니다.

1. [vercel.com](https://vercel.com)에서 이 저장소를 New Project로 가져옵니다(Import Git Repository).
2. **Framework Preset**을 `Other`로 선택합니다.
3. **Root Directory**는 저장소 루트(`/`)를 그대로 둡니다. Build Command / Output Directory는 비워둬도 됩니다.
4. **Deploy**를 누르면 `index.html`이 그대로 서빙됩니다.

로컬에서 미리 보려면 저장소 루트에서 아래 명령 중 하나를 실행한 뒤 브라우저로 열면 됩니다.

```bash
python3 -m http.server 8000
# 이후 http://localhost:8000 접속
```
