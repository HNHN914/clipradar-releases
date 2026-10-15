# ClipRadar 배포판

방송 녹화본에서 하이라이트를 찾아 쇼츠·클립으로 만드는 ClipRadar의 **배포판과 업데이트 정보**를 두는 곳입니다. 소스 코드는 비공개 저장소에 있습니다.

## 받기

[Releases](https://github.com/HNHN914/clipradar-releases/releases/latest)에서 `ClipRadar-win-x64-<버전>.zip`을 받아 압축을 풀고 `ClipRadar.exe`를 실행하세요(Windows 10/11 64비트).

- 이미 쓰고 있다면: ClipRadar를 종료(작업 표시줄 트레이 아이콘 → 종료)한 뒤 새 폴더로 바꾸면 됩니다. 프로젝트·영상·설정은 `%APPDATA%\ClipRadar`에 있어 그대로 남습니다.
- 0.2.0부터는 앱 안에서 새 버전 알림이 뜨고, **지금 업데이트**로 받아서 적용할 수 있습니다.

## 이 저장소의 파일

- `latest.json` — 앱이 새 버전을 확인할 때 읽는 파일(버전, 바뀐 점, zip 주소·크기·SHA-256, 서명). 배포할 때 `pnpm release:manifest`로 만든 파일로 교체합니다.
- Releases — 버전별 zip(태그 `v<버전>`). **zip을 먼저 올리고, 그다음 `latest.json`을 바꿉니다.**

배포 절차는 소스 저장소의 `docs/RELEASING.md`를 보세요.
