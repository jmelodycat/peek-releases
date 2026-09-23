# Peek

Five slots on the edge of your screen. Web pages, programs, files and folders open from one place.

[English](#english) · [한국어](#한국어)

This repository holds the installers only. The source is kept separately.

---

## English

Everything you open every day is scattered across bookmarks, the desktop and the file explorer. Peek gathers it into five slots so you stop hunting for things.

### Download

Get the latest build from [Releases](../../releases).

| | File | Requirements |
|---|---|---|
| Windows | `Peek_x.y.z_x64-setup.exe` | Windows 10 or later, 64-bit |
| macOS | `Peek_x.y.z_aarch64.dmg` | Apple silicon |

### Install

**Windows.** The installer shows an "unknown publisher" warning. This is a personal tool without code signing. Choose More info, then Run.

**macOS.** Open the dmg, move Peek to Applications, then right-click the icon and choose Open. A plain double-click will not work, for the same reason: no signing or notarisation. If it still refuses, run `xattr -cr /Applications/Peek.app` once in Terminal.

The how-to window opens once after installing. You can reopen it any time from the tray icon. Installing a newer build over an older one keeps the five slots you set up.

### Three things worth knowing

**Adding.** Drop web pages, programs and folders straight onto a slot. Dragging a link from your browser works too. Or click an empty slot and type an address or a path.

**Grouping.** Drop an icon onto the middle of another slot to group them. Let go once the border appears. A slot holds up to four, and clicking it opens them all in order. Group the things you always start your morning with and one button does the lot. The button at the top left of a group opens the list inside, where you can take items out or break the group apart.

**Tidying up.** The down arrow folds the widget away and leaves a single handle. Windows key + D folds it with everything else and unfolds it again (Windows only). Drag the three dots to move it, and it snaps to the edge of the screen. Drag a slot onto the top or bottom edge of another to reorder.

### Everything else

| Action | What it does |
|---|---|
| Right-click a slot | Change its name and address |
| Hover over a slot | Red X to delete |
| Right-click the panel | Theme, colour, language, character, start-up, how to use, quit |
| Tray icon | Show widget, move to centre, how to use, quit |

Every setting lives in the panel's right-click menu. The menu stays open after you pick something, so you can try things side by side.

Colours are the six dots in the middle of the menu: default, pink, blue, green, violet and sand. Light and dark are calculated separately from the colour you choose.

Peek speaks Korean and English. It follows your system language, and you can pin one in the menu.

There are five characters. None is the default, and they move now and then.

| | Characters |
|---|---|
| Disappears when folded | Crocodile, dinosaur |
| Stays when folded | Cat, tabby, resting crocodile |

Lost the widget? Use the tray icon and choose Move to centre.

### Opening with a shortcut

Right-click a group to open its list. At the bottom, choose Set a shortcut and press the key you want. Ctrl + Alt is added for you. If another program already uses that combination, Peek tells you instead of taking it.

Other tools can call Peek with this address.

```
peek://open/<slot or group name>
```

It starts the app if it is not running. The name has to match exactly.

### Privacy

What you add and how you use it never leaves this computer. There is no account and no server sync. Only two things reach the network: fetching the icon for a web address, and asking whether a newer version exists. Neither request sends anything about you.

Settings are kept in one file.

```
Windows  %APPDATA%\dev.jmelodycat.peekwidget\config.json
macOS    ~/Library/Application Support/dev.jmelodycat.peekwidget/config.json
```

### Uninstalling

On Windows, remove Peek from Settings > Apps > Installed apps. On macOS, delete Peek.app from Applications. The settings file stays at the path above, so delete that folder as well if you want it gone.

### Reporting something

Please open an [issue](../../issues). This is made by one person, so replies can be slow.

---

## 한국어

매일 여는 것들이 즐겨찾기, 바탕화면, 탐색기에 흩어져 있어 찾는 데 드는 시간을 없애려고 만들었습니다. 웹페이지, 프로그램, 파일, 폴더를 모두 다섯 칸에 모읍니다.

### 받기

[Releases](../../releases) 에서 최신 판을 받으세요.

| | 파일 | 요구 사항 |
|---|---|---|
| 윈도우 | `Peek_x.y.z_x64-setup.exe` | 윈도우 10 이상, 64비트 |
| 맥 | `Peek_x.y.z_aarch64.dmg` | 애플 실리콘 |

### 설치

**윈도우.** 설치 파일을 실행하면 "게시자를 알 수 없습니다" 경고가 뜹니다. 코드 서명을 하지 않은 개인 도구라 그렇습니다. 추가 정보를 누르고 실행을 고르면 설치됩니다.

**맥.** dmg를 열어 응용 프로그램으로 옮긴 뒤, 아이콘을 오른쪽 클릭해서 열기를 고릅니다. 그냥 두 번 눌러서는 열리지 않습니다. 이것도 서명과 공증을 하지 않아서입니다. 계속 막히면 터미널에서 `xattr -cr /Applications/Peek.app` 을 한 번 실행하세요.

설치가 끝나면 사용법 창이 한 번 뜹니다. 트레이 아이콘에서 언제든 다시 열 수 있습니다. 다음 판을 덮어 설치해도 등록해 둔 다섯 칸은 그대로 남습니다.

### 세 가지만 알면 됩니다

**넣기.** 웹페이지, 프로그램, 폴더 모두 칸에 끌어다 놓으면 들어갑니다. 브라우저에서 링크를 그대로 끌어와도 됩니다. 빈 칸(+)을 눌러 주소나 경로를 직접 넣어도 됩니다.

**묶기.** 아이콘을 다른 칸 한가운데에 올려놓으면 묶입니다. 테두리가 생겼을 때 놓으세요. 한 칸에 4개까지 들어갑니다. 묶인 칸을 누르면 담긴 것이 순서대로 전부 열립니다. 아침에 늘 같이 켜는 것들을 묶어두면 버튼 하나로 끝납니다. 묶음 왼쪽 위의 버튼을 누르면 담긴 목록이 열리고, 거기서 하나씩 빼거나 묶음째 풀 수 있습니다.

**정리.** 아래 화살표를 누르면 접힙니다. 손잡이 한 줄만 남습니다. 윈도우키 + D를 누르면 같이 접히고, 다시 누르면 같이 펴집니다(윈도우만). 점 세 개를 끌면 옮겨지고 화면 가장자리에 붙습니다. 칸을 끌어 다른 칸의 위나 아래 끄트머리에 놓으면 순서가 바뀝니다.

### 그 밖에

| 조작 | 하는 일 |
|---|---|
| 칸 오른쪽 클릭 | 이름과 주소 고치기 |
| 칸에 마우스 올리기 | 빨간 X로 지우기 |
| 패널 오른쪽 클릭 | 테마, 색, 언어, 캐릭터, 자동 실행, 사용법, 종료 |
| 트레이 아이콘 | 위젯 보이기, 화면 중앙으로, 사용법, 종료 |

설정은 전부 패널 오른쪽 클릭에 있습니다. 메뉴는 고른다고 닫히지 않아서 하나씩 눌러 보며 정할 수 있습니다.

색은 메뉴 가운데 점 여섯 개입니다. 기본, 핑크, 파랑, 초록, 보라, 모래 중에 고릅니다. 고른 색에 맞춰 라이트와 다크가 각각 따로 계산됩니다.

한국어와 영어로 씁니다. 운영체제 언어를 따라가고, 메뉴에서 하나로 고정할 수도 있습니다.

캐릭터는 다섯입니다. 기본은 캐릭터 없음이고, 가끔 움직임이 있습니다.

| | 캐릭터 |
|---|---|
| 접으면 같이 사라짐 | 악어, 공룡 |
| 접어도 남음 | 고양이, 얼룩 고양이, 엎드린 악어 |

위젯을 잃어버렸으면 트레이 아이콘에서 화면 중앙으로를 누르세요.

### 단축키로 열기

묶음을 오른쪽 클릭하면 목록이 열립니다. 맨 아래 단축키 걸기를 누르고 원하는 글자를 누르세요. Ctrl + Alt는 자동으로 붙습니다. 이미 다른 프로그램이 쓰는 키면 걸리지 않고 알려줍니다.

다른 도구에서 부르려면 이 주소를 쓰면 됩니다.

```
peek://open/<칸이나 묶음 이름>
```

앱이 꺼져 있어도 켜지면서 엽니다. 등록해 둔 이름과 정확히 맞아야 열립니다.

### 개인 정보

등록한 주소와 사용 기록은 이 컴퓨터 밖으로 나가지 않습니다. 계정도 서버 동기화도 없습니다. 밖으로 나가는 것은 두 가지뿐입니다. 웹 주소의 아이콘을 가져올 때와, 새 판이 나왔는지 물을 때입니다. 둘 다 보내는 값이 없습니다.

설정은 아래 한 파일에만 저장됩니다.

```
윈도우  %APPDATA%\dev.jmelodycat.peekwidget\config.json
맥      ~/Library/Application Support/dev.jmelodycat.peekwidget/config.json
```

### 지우기

윈도우는 설정 > 앱 > 설치된 앱에서 Peek을 제거합니다. 맥은 응용 프로그램에서 Peek.app을 지웁니다. 설정 파일은 위 경로에 남으므로 필요하면 폴더째 지우세요.

### 알려주기

버그나 불편한 점은 [Issues](../../issues) 에 남겨주세요. 혼자 만드는 도구라 답이 늦을 수 있습니다.
