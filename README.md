# Nyang Nap 다운로드

가민 Forerunner 265 / 265S 용 도트 고양이 워치페이스 **냥냅**과 달리기 데이터 필드 **냥런**의 설치 파일을 받는 곳입니다. 소스는 여기 없고 배포 파일만 올라옵니다.

## 받기

최신 버전: https://github.com/yonadora/nyang-nap-releases/releases/latest

| 기기 | 파일 |
|---|---|
| Forerunner 265 | `NyangNap_<버전>.zip` |
| Forerunner 265S | `NyangNap_<버전>_fr265s.zip` |

압축을 풀면 `NyangNap.prg` 하나가 나옵니다.

## 설치

시계를 USB 로 연결하고(잠금 해제) 시계 안 `GARMIN/APPS/` 폴더에 `NyangNap.prg` 를 넣습니다. 이미 있으면 교체합니다.
`GARMIN/APPS/SETTINGS/` 안의 `.SET` 파일은 지우지 마세요. 설정(고양이·줄 구성·배치 등)이 들어 있습니다.

- **Windows**: 탐색기에서 시계(Forerunner) → Internal Storage → GARMIN → APPS 로 끌어다 놓기.
- **Mac**: macOS 는 MTP 를 기본 지원하지 않아 [OpenMTP](https://openmtp.ganeshrvel.com/) 로 시계를 열어 같은 폴더에 넣습니다. Garmin Express 가 켜져 있으면 끄세요.

USB 를 뽑으면 시계가 워치페이스를 다시 읽습니다. 시계에서 UP 길게 → 시계 모드 → Nyang Nap 을 고르고, 설정 메뉴 맨 아래 **Build** 줄로 버전을 확인할 수 있습니다.

## 설정

USB 로 넣은 앱은 Garmin Connect 폰 앱에 설정 화면이 뜨지 않습니다. 설정은 시계 안 메뉴(시계 모드 → Nyang Nap → 설정)에서 합니다:
Version(하단 두 줄) / Cat(고양이) / Time(24h·12h) / Layout(Flat·Round) / Rows(오른쪽 열 항목) / Hours(시간대 경계).

## 냥런 (Nyang Run)

달리기(Run) 활동용 **데이터 필드**입니다. 고양이가 나 자신이고, 트랙 한 줄이 목표 거리, 표정·땀방울·속도선이 목표 페이스와의 차이를 보여 줍니다.

**받기**: [Releases](https://github.com/yonadora/nyang-nap-releases/releases) 에서 제목이 **Nyang Run** 인 릴리즈(가장 위의 것)를 엽니다. (위의 "최신 버전" 링크는 냥냅 워치페이스입니다)

| 기기 | 파일 |
|---|---|
| Forerunner 265 | `NyangPacer_<버전>.zip` |
| Forerunner 265S | `NyangPacer_<버전>_fr265s.zip` |

**설치**: 냥냅과 같습니다. 압축을 풀어 나온 `NyangPacer.prg` 를 이름 그대로 시계의 `GARMIN/APPS/` 에 넣습니다(Mac 은 OpenMTP). `SETTINGS/NyangPacer.SET` 은 지우지 마세요.

**쓰기**: 달리기 활동 → UP 길게 → 달리기 설정 → 데이터 화면 → 새로 추가(또는 기존 화면) → 배치 **1칸** → Connect IQ 필드 → **Nyang Run**.
설정(고양이·목표 페이스·목표 거리)은 그 데이터 필드의 설정 메뉴에서 합니다. 기본값은 짜브 · 5:40/km · 5km 입니다.

## 건의 · 문제 신고

바꾸고 싶은 점이나 이상한 동작은 [Issues](https://github.com/yonadora/nyang-nap-releases/issues/new/choose) 에 올려 주세요. "건의 / 기능 요청"과 "문제 신고" 양식이 있습니다. 글을 쓰려면 GitHub 계정(무료)이 필요하고, 다운로드는 계정 없이 됩니다.
