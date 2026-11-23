---
layout: page
title: 第三者ライセンス
---

**対象: HamonPlayer 1.0.6（Windows 版。Microsoft Store 版・setup.exe 版）**

HamonPlayer には、次の第三者ソフトウェアが含まれています。それぞれの提供者が定める条件が適用されます。以下に、ライセンスが求める表示を掲げます。

- **NAudio.Core、NAudio.Wasapi** — 版: 2.2.1 / ライセンス: MIT / 提供者: Mark Heath / <https://github.com/naudio/NAudio>
- **Vortice.MediaFoundation、Vortice.DirectX** — 版: 3.8.3 / ライセンス: MIT / 提供者: Amer Koleci and Contributors / <https://github.com/amerkoleci/Vortice.Windows>
- **Vortice.Mathematics** — 版: 2.1.0 / ライセンス: MIT / 提供者: Amer Koleci and Contributors / <https://github.com/amerkoleci/Vortice.Mathematics>
- **SharpGen.Runtime、SharpGen.Runtime.COM** — 版: 2.4.2-beta / ライセンス: MIT / 提供者: Alexandre Mutel、Jeremy Koritzinsky、Amer Koleci / <https://github.com/SharpGenTools/SharpGenTools>
- **.NET ランタイムおよびライブラリ** — 版: 10.0 / ライセンス: MIT、.NET Library License / 提供者: Microsoft Corporation / <https://dotnet.microsoft.com/>
- **Windows SDK の .NET 向けの部品（Microsoft.Windows.SDK.NET、WinRT.Runtime）** — 版: 10.0.19041.57 / ライセンス: Microsoft Windows SDK のライセンス条項 / 提供者: Microsoft Corporation / <https://aka.ms/WinSDKLicenseURL>
- **Inno Setup**（setup.exe 版のインストーラとアンインストーラだけ） — 版: 6.6.1 / ライセンス: Inno Setup License / 提供者: Jordan Russell、Martijn Laan / <https://jrsoftware.org/>

HamonPlayer の Windows 版は、これ以外のパッケージ（外部のライブラリ）を使っていません。スマホ版（Android）に含まれるものは、スマホ版を出すときに足します。

---

## NAudio.Core、NAudio.Wasapi

ほかのアプリが音を出しているかを見るために使っています（ほかのアプリが音を出したら一時停止するため）。

```
© Mark Heath 2023

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## Vortice.MediaFoundation、Vortice.DirectX、Vortice.Mathematics

Windows の再生の仕組み（Media Foundation）で、曲を鳴らし、動画を映し、曲の音の大きさを測るために使っています。

```
Copyright (c) Amer Koleci and Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## SharpGen.Runtime、SharpGen.Runtime.COM

上の Vortice が、Windows の部品を呼ぶために使っています。

```
(c) 2010-2017 Alexandre Mutel, 2017-2023 Jeremy Koritzinsky, 2023-2024 Amer Koleci

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## .NET ランタイムおよびライブラリ

HamonPlayer は .NET 10 で作られており、**実行に必要な .NET のランタイムとライブラリを同梱しています**（自己完結型）。そのため、利用者が別途 .NET を入れる必要はありません。

.NET のソースコードは、次の MIT ライセンスで公開されています。

```
The MIT License (MIT)

Copyright (c) .NET Foundation and Contributors

All rights reserved.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

同梱するランタイムの再頒布には .NET Library License（<https://dotnet.microsoft.com/dotnet_library_license.htm>）が適用されます。これに従い、利用条件 §7 に、Microsoft と .NET を保護する条項を置いています。要点は次のとおりです。

- Microsoft は .NET について**いかなる保証も行わず**、いかなる損害についても責任を負いません。
- 利用者は .NET を、リバースエンジニアリング、逆コンパイル、逆アセンブルしないものとします（適用される法令がこれを明示的に認める範囲を除きます）。
- HamonPlayer を再配布する場合は、**受け取る人にも、Microsoft と .NET を同等以上に保護する条件に同意してもらう**必要があります。

---

## Windows SDK の .NET 向けの部品（Microsoft.Windows.SDK.NET、WinRT.Runtime）

Windows の部品を呼ぶために使っています（今の曲の名前とジャケットの絵を Windows のメディアの欄に出し、キーボードのメディアキーを受ける。曲のタグを読む。Store 版で、Windows の起動時の起動を入れ / 切りする）。

これらは、Microsoft の再頒布の一覧（「Windows SDK redist lists」<https://learn.microsoft.com/en-us/legal/windows-sdk/redist> の「Microsoft.Windows.SDK.NET.Ref」）に載っている部品で、Windows の部品を呼ぶためにアプリの一部として、変えずに配っています。これらの再頒布には、Microsoft Windows SDK のライセンス条項（「MICROSOFT SOFTWARE LICENSE TERMS — MICROSOFT WINDOWS SOFTWARE DEVELOPMENT KIT (SDK) FOR WINDOWS 10」。<https://aka.ms/WinSDKLicenseURL>）が適用されます。この条項は、受け取る人に、これらを同等以上に保護する条件に同意してもらうことを求めています。これに従い、利用条件 §7 に、Microsoft とこれらを保護する条項を置いています。

---

## Inno Setup

setup.exe 版のインストーラとアンインストーラに使っています。Microsoft Store 版には含まれません。

```
Inno Setup License
==================

Except where otherwise noted, all of the documentation and software included in the Inno
Setup package is copyrighted by Jordan Russell.

Copyright (C) 1997-2025 Jordan Russell. All rights reserved.
Portions Copyright (C) 2000-2025 Martijn Laan. All rights reserved.

This software is provided "as-is," without any express or implied warranty. In no event shall
the author be held liable for any damages arising from the use of this software.

Permission is granted to anyone to use this software for any purpose, including commercial
applications, and to alter and redistribute it, provided that the following conditions are met:

1. All redistributions of source code files must retain all copyright notices that are currently
   in place, and this list of conditions without modification.

2. All redistributions in binary form must retain all occurrences of the above copyright notice
   and web site addresses that are currently in place (for example, in the About boxes).

3. The origin of this software must not be misrepresented; you must not claim that you wrote
   the original software. If you use this software to distribute a product, an acknowledgment
   in the product documentation would be appreciated but is not required.

4. Modified versions in source or binary form must be plainly marked as such, and must not
   be misrepresented as being the original software.


Jordan Russell
jr-2020 AT jrsoftware.org
https://jrsoftware.org/
```

---

## この表示について

HamonPlayer が使うソフトウェアを増やしたり、版を上げたりしたときは、この文書を改めます。抜けや誤りに気づかれたときは、問い合わせ窓口（<https://github.com/poola-vii/support>）へお知らせください。

© 2026 poola-vii
