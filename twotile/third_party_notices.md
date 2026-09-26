---
layout: page
title: 第三者ライセンス
---

**対象: TwoTile 1.0.1（Microsoft Store 版・ポータブル版）**

> **準備中です。まだ配っていません。** TwoTile はこれから無料の公開βとして出します。公開したときに、この注記を外します。 同梱するものが確定したときに、この表示を最終化します。

TwoTile には、次の第三者ソフトウェアが含まれています。それぞれの提供者が定める条件が適用されます。以下に、各ライセンスが求める表示を掲げます。

| ソフトウェア | 版 | ライセンス | 提供者 |
|:---|:---|:---|:---|
| [Markdig](https://xoofx.github.io/markdig) | 1.0.0 | BSD 2-Clause | Alexandre Mutel |
| [Microsoft.Web.WebView2](https://aka.ms/webview) | 1.0.3800.47 | BSD 3-Clause | Microsoft Corporation |
| [Microsoft.Extensions.DependencyInjection](https://dot.net/) | 10.0.5 | MIT | Microsoft Corporation |
| [.NET ランタイムおよびライブラリ](https://dotnet.microsoft.com/) | 10.0 | MIT / .NET Library License | Microsoft Corporation |

---

## Markdig

ユーザマニュアルの Markdown を HTML へ変換するために使っています。

```
Copyright (c) 2018-2019, Alexandre Mutel
All rights reserved.

Redistribution and use in source and binary forms, with or without modification
, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

---

## Microsoft.Web.WebView2

アプリ内のヘルプ画面を表示するために使っています。

```
Copyright (C) Microsoft Corporation. All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are
met:

   * Redistributions of source code must retain the above copyright
notice, this list of conditions and the following disclaimer.
   * Redistributions in binary form must reproduce the above
copyright notice, this list of conditions and the following disclaimer
in the documentation and/or other materials provided with the
distribution.
   * The name of Microsoft Corporation, or the names of its contributors
may not be used to endorse or promote products derived from this
software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

WebView2 ランタイム本体は Windows に付属するもので、TwoTile には含まれません。

---

## Microsoft.Extensions.DependencyInjection

アプリ内部の部品を組み立てるために使っています。

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

---

## .NET ランタイムおよびライブラリ

TwoTile は .NET 10 で作られており、**実行に必要な .NET のランタイムとライブラリを同梱しています**（自己完結型）。そのため、利用者が別途 .NET を入れる必要はありません。

.NET のソースコードは MIT ライセンスで公開されています。上の Microsoft.Extensions.DependencyInjection と同じ文面です（`Copyright (c) .NET Foundation and Contributors`）。

同梱するランタイムの再頒布には [.NET Library License](https://dotnet.microsoft.com/dotnet_library_license.htm) が適用されます。これに従い、[利用条件](terms.md) §7 に、Microsoft と .NET を保護する条項を置いています。要点は次のとおりです。

- Microsoft は .NET について**いかなる保証も行わず**、いかなる損害についても責任を負いません。
- 利用者は .NET を、リバースエンジニアリング、逆コンパイル、逆アセンブルしないものとします（適用される法令がこれを明示的に認める範囲を除きます）。
- TwoTile を再配布する場合は、**受け取る人にも、Microsoft と .NET を同等以上に保護する条件に同意してもらう**必要があります。

---

## この表示について

TwoTile が使っているパッケージを増やしたり、版を上げたりしたときは、この文書を改めます。抜けや誤りに気づかれたときは[問い合わせ窓口](support.md)へお知らせください。

TwoTile 本体の利用条件は[利用条件](terms.md)をご覧ください。

© 2026 poola-vii
