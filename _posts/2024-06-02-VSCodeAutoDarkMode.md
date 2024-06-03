---
title: Visual Studio Code 자동 다크모드.md
date: 2024-06-02 21:37:43 +09:00
categories: util
tags: vscode utils theme automation
---

VSCode를 사용하면 대부분 시력 보호를 위해 다크모드를 사용한다.
자연광과 등불로 주변이 밝으면 오히려 다크 모드가 코드를 읽는 데 방해가 된다.
VSCode는 Windows의 색 테마와 연동하여 테마를 바꿀 수 있다.
VSCode 설정을 아래와 같이 바꿔주면 알아서 바꿔준다.
Windows의 테마를 일몰, 일출 시간에 따라 바꿔주는 설정은 [이곳]({% post_url 2024-06-02-WindowsAutoDarkMode %})을 확인하면 된다.

```json
{
  "window.autoDetectColorScheme": true,
  "workbench.preferredLightColorTheme": "" /*사용할 밝은 테마의 이름*/,
  "workbench.preferredDarkColorTheme": "" /*사용할 어두운 테마의 이름*/
}
```
