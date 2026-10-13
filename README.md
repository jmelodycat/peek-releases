# Peek

윈도우와 맥에서 쓰는 바탕화면 런처 위젯입니다. 화면 가장자리에 아이콘을 최대 5개까지 두고 웹페이지, 프로그램, 파일, 폴더를 한곳에서 엽니다. 맥에서는 메뉴 막대에 둘 수도 있습니다.
A desktop launcher and dock for Windows and macOS. Up to five icons at the edge of your screen open web pages, programs, files and folders from one place. On a Mac, Peek can also sit under the menu bar.

[한국어](#한국어) · [English](#english)

이 저장소에는 설치 파일만 있습니다. 소스 코드는 공개하지 않습니다.
This repository holds installers only. The source code is not public.

---

## 한국어

<img src="images/first-run.png" width="388" alt="화면 오른쪽에 나타난 Peek 위젯과 지금 열어 둔 것에서 넣기 화면">

### 다운로드와 설치

[Releases](../../releases)에서 최신 버전을 받습니다.

| 운영체제 | 파일 | 요구 사항 |
|---|---|---|
| 윈도우 | `Peek_x.y.z_x64-setup.exe` | 윈도우 10 이상, 64비트 |
| 맥 | `Peek_x.y.z_universal.dmg` | 애플 실리콘과 인텔 모두 |

- **윈도우.** 개인이 만든 프로그램이라 코드 서명이 없어 "게시자를 알 수 없습니다" 경고가 나옵니다. 추가 정보를 클릭한 뒤 실행을 선택하면 설치됩니다.
- **맥.** dmg를 열어 Peek을 응용 프로그램 폴더로 옮깁니다. 서명이 없어 열리지 않으면 터미널에서 `xattr -cr /Applications/Peek.app`을 한 번 실행합니다.

새 버전을 덮어 설치해도 넣어 둔 아이콘은 유지됩니다.

### 사용법

<img src="images/group.png" width="191" align="right" alt="그룹과 웹 주소가 들어 있는 Peek 위젯">

처음 실행하면 실행 중인 프로그램과 열린 폴더, 브라우저 탭 목록이 먼저 표시됩니다. 미리 선택된 3개를 확인하고 넣기를 클릭하면 위젯에 추가됩니다.

- **넣기.** 웹페이지, 프로그램, 폴더를 + 위로 끌어다 놓거나 +를 클릭해 주소를 입력합니다.
- **고치기와 지우기.** 아이콘에 마우스를 올리면 연필(고치기)과 빨간 X(지우기) 버튼이 나타납니다.
- **그룹.** 아이콘을 다른 아이콘 가운데에 놓으면 그룹으로 묶입니다. 그룹을 클릭하면 담긴 항목이 최대 4개까지 한 번에 열리고, 그룹의 연필 버튼에서 Ctrl + Alt 단축키를 지정할 수 있습니다.
- **접기와 옮기기.** 아래쪽 화살표로 접고, 아이콘이 없는 곳을 잡아 끌어 옮깁니다. 윈도우에서는 Windows 키 + D로 다른 창과 함께 감춰집니다.
- **설정.** 점 세 개 메뉴에서 테마, 색, 언어, 캐릭터, 자동 실행을 바꾸고 자세한 사용법을 엽니다.

다른 프로그램에서는 `peek://open/<아이콘 또는 그룹 이름>` 주소로 아이콘이나 그룹을 열 수 있습니다.

<br clear="right">

### 맥 메뉴 막대

<img src="images/menubar.png" width="312" align="right" alt="맥 메뉴 막대의 Peek 아래에 열린 목록">

맥에서 처음 설치하면 Peek이 메뉴 막대 아이콘 아래에 목록으로 표시됩니다. ⌥Space로 열고, 점 세 개 메뉴 맨 위의 "보이는 곳"에서 가장자리 방식으로 바꿀 수 있습니다.

Safari 탭과 Finder 폴더를 목록에 보여 주기 위해 처음에 자동화 권한을 요청합니다. 허용하지 않아도 나머지 기능은 그대로 사용할 수 있습니다.

<br clear="right">

### 개인 정보

넣어 둔 주소와 사용 기록은 컴퓨터 밖으로 전송되지 않습니다. 계정과 서버 동기화가 없습니다. 외부와 통신하는 경우는 웹 주소의 아이콘을 가져올 때와 새 버전을 확인할 때뿐이며, 사용자 정보는 보내지 않습니다. 설정은 아래 파일 한 개에 저장됩니다.

```
윈도우  %APPDATA%\app.peekwidget\config.json
맥      ~/Library/Application Support/app.peekwidget/config.json
```

### 삭제와 문의

윈도우는 설정 > 앱 > 설치된 앱에서, 맥은 응용 프로그램 폴더에서 Peek을 삭제합니다. 설정까지 지우려면 위 경로의 폴더도 삭제합니다.

버그나 불편한 점은 [Issues](../../issues)에 올려 주세요. 개인이 만든 프로그램이라 답변이 늦을 수 있습니다.

---

## English

### Download and install

Get the latest version from [Releases](../../releases).

| OS | File | Requirements |
|---|---|---|
| Windows | `Peek_x.y.z_x64-setup.exe` | Windows 10 or later, 64-bit |
| macOS | `Peek_x.y.z_universal.dmg` | Apple Silicon and Intel |

- **Windows.** Peek is a personal project without a code signature, so Windows shows "Unknown publisher". Click More info, then Run anyway.
- **macOS.** Open the dmg and move Peek to Applications. Peek is not signed, so if it won't open, run `xattr -cr /Applications/Peek.app` in Terminal once.

Installing a new version over the old one keeps your icons.

### How to use

<img src="images/group.png" width="191" align="right" alt="The Peek widget with a group and a web address">

On first launch, Peek shows a list of running programs, open folders and browser tabs. Check the three preselected items and click Add to put them in the widget.

- **Add.** Drag a web page, program or folder onto +, or click + and type an address.
- **Edit and remove.** Hover over an icon to see the pencil (edit) and the red X (remove).
- **Groups.** Drop an icon onto the center of another to group them. Clicking a group opens everything in it, up to four items. Set a Ctrl + Alt shortcut from the group's pencil button.
- **Fold and move.** Click the arrow at the bottom to fold. Drag anywhere except an icon to move the widget. On Windows, Windows key + D hides it along with other windows.
- **Settings.** The three-dot menu changes the theme, color, language, character and startup option, and opens the full guide.

Other programs can open an icon or group with `peek://open/<icon or group name>`.

<br clear="right">

### macOS menu bar

On a Mac, a new install shows Peek as a list under its menu bar icon. Press ⌥Space to open it. Switch to edge mode under "Show in" at the top of the three-dot menu.

Peek asks for Automation permission on first launch to list Safari tabs and Finder folders. Everything else works if you decline.

### Privacy

Your addresses and usage history never leave your computer. There is no account and no server sync. Peek connects to the internet only to fetch website icons and to check for new versions, and it sends no user information. Settings are stored in one file.

```
Windows  %APPDATA%\app.peekwidget\config.json
macOS    ~/Library/Application Support/app.peekwidget/config.json
```

### Uninstall and feedback

On Windows, remove Peek from Settings > Apps > Installed apps. On a Mac, delete Peek.app from Applications. To remove your settings too, delete the folder in the path above.

Report bugs or problems in [Issues](../../issues). Peek is a personal project, so replies may take a while.
