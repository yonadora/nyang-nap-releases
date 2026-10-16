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
설정(고양이·목표 페이스·목표 거리·Unlock)은 달리기 화면에서 **UP 길게 → 활동 메뉴 → Nyang Run** 에서 엽니다(데이터 화면 편집 쪽에서는 열리지 않습니다). 기본값은 짜브 · 5:40/km · 5km 입니다.

## 무료 체험 · 언락코드

냥냅 1.1.16, 냥런 0.4.20 부터 **7일 무료 체험** 뒤 언락코드로 계속 쓰는 방식입니다.

- 처음 실행한 날부터 7일 동안 모든 기능을 씁니다(오래된 버전을 늦게 받으면 짧아질 수 있지만 최소 3일). 마지막 2일은 남은 날(예: 2D)이 보입니다(냥런, 냥냅은 Flat 배치).
- 체험이 끝나면 잠깁니다. 냥냅은 시간만 보이고 다른 값 자리에 자물쇠, 냥런은 현재 페이스·거리·시간만 보입니다. 잠긴 화면에 내 **Device ID** 가 나옵니다(냥런은 타이머가 멈췄을 때).
- **Device ID 확인**: 냥냅은 시계 모드 → Nyang Nap → 설정 → **Unlock → Device ID**, 냥런은 달리기 화면에서 UP 길게 → 활동 메뉴 → Nyang Run → **Unlock → Device ID**. 형식은 `ABCD-EFGH-K` 이고, 같은 시계라도 냥냅과 냥런의 ID 가 다릅니다.
- **언락코드 받기**: 아래 [Issues](https://github.com/yonadora/nyang-nap-releases/issues/new/choose) 에 앱 이름과 Device ID 를 적어 요청해 주세요. 받은 8자를 **Unlock → Enter Code** 에 넣으면 바로 풀리고 Status 가 **Unlocked** 가 됩니다. 코드는 그 시계·그 앱에서만 맞고, 다시 설치해도 그대로 쓸 수 있습니다.

## 건의 · 문제 신고

바꾸고 싶은 점이나 이상한 동작은 [Issues](https://github.com/yonadora/nyang-nap-releases/issues/new/choose) 에 올려 주세요. "건의 / 기능 요청"과 "문제 신고" 양식이 있습니다. 글을 쓰려면 GitHub 계정(무료)이 필요하고, 다운로드는 계정 없이 됩니다.
