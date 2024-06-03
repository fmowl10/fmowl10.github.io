---
title: Visual Studio Code 자동 다크모드.md
date: 2024-06-02 21:37:43 +09:00
categories: util
tags: vscode utils theme automation
---

VSCode를 사용하면 대부분 시력 보호를 위해 다크모드를 사용한다.
자연광과 등불로 주변이 밝으면 오히려 다크 모드가 코드를 읽는 데 방해가 된다.
이런 문제를 해결하기 위해 딱 일몰때 다크 모드로 바꿔주는 extension을 찾았다.
[Sundial](https://marketplace.visualstudio.com/items?itemName=muuvmuuv.vscode-sundial)은 자동으로 특정한 시간, 사용자의 위치에 따라 계산된 일몰시간, Windows의 테마에 따라 테마를 적절하게 바꿀 수 있다.
먼저 Sundial을 설치하고 설정창에서 먼저 2개의 값을 설정한다.
낮에 쓸 테마와 밤에 쓸 테마를 설정해주면 Sundial이 시간에 맞추어 바꿔준다.

```json
{
  "workbench.preferredLightColorTheme": "" /*사용할 밝은 테마의 이름*/,
  "workbench.preferredDarkColorTheme": "" /*사용할 어두운 테마의 이름*/
}
```

**sundial.autoLocale**를 이용해 위치 정보를 기준으로 바꿀 수 있다.
