# 컷콕 (CutKok) 배포판

**재밌는 순간만, 콕.** 방송 녹화본에서 재밌는 장면을 찾아 쇼츠·클립으로 쉽게 편집하는 컷콕의 **배포판과 업데이트 정보**를 두는 곳입니다. 소스 코드는 비공개 저장소에 있습니다.

## 받기

[Releases](https://github.com/HNHN914/cutkok-releases/releases/latest)에서 `CutKok-win-x64-<버전>.zip`을 받아 압축을 풀고 `CutKok.exe`를 실행하세요(Windows 10/11 64비트).

- `-update.zip`은 앱의 자동 업데이트용입니다. 직접 받을 필요는 없습니다.
- 이미 쓰고 있다면: 작업 표시줄 트레이 아이콘 → 종료한 뒤 새 폴더로 바꾸면 됩니다. 프로젝트·영상·설정은 `%APPDATA%\CutKok`에 있어 그대로 남습니다.
- 앱 안에서 새 버전 알림이 뜨고, **지금 업데이트**로 받아서 적용할 수 있습니다.

### 예전 이름(ClipRadar)을 쓰던 분

컷콕의 이전 이름은 ClipRadar입니다(0.2.0까지).

- 0.2.0에서도 자동 업데이트는 그대로 됩니다.
- 이름과 아이콘까지 바꾸려면 ClipRadar를 종료하고 새 zip의 `CutKok.exe`를 실행하세요. `%APPDATA%\ClipRadar`의 프로젝트·설정은 처음 실행할 때 자동으로 옮겨집니다.
- 이 저장소의 예전 주소(`clipradar-releases`)는 GitHub가 자동으로 연결합니다.

## 이 저장소의 파일

- `latest.json` — 앱이 새 버전을 확인할 때 읽는 파일(버전, 바뀐 점, zip 주소·크기·SHA-256, 서명). 배포할 때 `pnpm release:manifest`로 만든 파일로 교체합니다. 서명돼 있으니 손으로 고치지 마세요.
- Releases — 버전별 zip(태그 `v<버전>`). **zip을 먼저 올리고, 그다음 `latest.json`을 바꿉니다.**

배포 절차는 소스 저장소의 `docs/RELEASING.md`를 보세요.
