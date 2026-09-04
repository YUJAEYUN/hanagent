# 하나증권 CI 자산

출처: https://github.com/YUJAEYUN/hana_securities_ppt_design (main)

사용한 원본 커밋: `8f3db100279c910e9d4660a933b313320cf9a2e9`.

- `brand/HanaSecurities_logo-lockup.png`: `hana-ppt-skill/assets/logo/`의 심볼+워드마크 PNG 원본. 색·비율·알파 채널을 바꾸지 않고 흰 배경에 사용합니다.
- `brand/HanaSecurities_symbol-mark.png`: 같은 저장소의 심볼 PNG 원본. 파비콘으로 사용합니다.
- `fonts/Hana2-{Regular,Medium,Bold,Heavy}.woff2`: `hana-ppt-skill/assets/fonts/windows/Hana2.0_TTF.zip`의 동명 TTF를 fontTools로 WOFF2 압축했습니다. 글리프 서브셋·윤곽 수정 없이 전체 문자와 이름·저작권 메타데이터를 보존합니다. 원본은 저장소에 보관되어 있습니다.

본문은 Regular(400), 본문 강조는 Medium(500), 섹션 제목은 Bold(700), 첫 화면 제목은 Heavy(900)를 사용합니다. 한글 코드 자료에는 Consolas 다음으로 하나2.0을 지정합니다. 시스템 폰트 설치나 외부 CDN 요청은 필요하지 않습니다.

색상 정본: `hana-ppt-skill/assets/ci-colors.json`의 HEX 값입니다.

| 역할 | 값 |
| --- | --- |
| Hana Green | `#009178` |
| Hana Dark Green | `#004E42` |
| Hana Red | `#DC231E` |
| Hana Pale Green | `#DBEDE7` |
| Hana Light Green | `#A7D8B8` |

본문 잉크·구분선·종이 배경에 쓰는 보조 중립색은 웹 가독성을 위해 별도로 정한 값입니다. PPT의 pt 수치를 웹의 px로 복제하지 않고 반응형 rem 크기로 적용했습니다. 로고 보호영역·최소 크기는 출처에서도 미확정이므로 이 페이지의 여백을 공식 규정이라고 주장하지 않습니다. 임의 심볼, 로고 재색칠, 어두운 배경용 반전 로고는 사용하지 않습니다.

## 배포

`index.html`과 `assets/`를 같은 위치에 함께 배포해야 합니다. 기존처럼 빌드 없이 정적 파일로 제공하면 됩니다. HTML 파일만 별도로 복사하면 로고와 웹폰트 경로가 끊어집니다.
