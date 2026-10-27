---
layout: page
title: Third-Party Notices
lang: en
---

**Applies to: TwoTile 1.0.9 (Microsoft Store version and portable version)**

TwoTile includes the following third-party software. Each is subject to the terms set by its provider. The notices each license requires are shown below.

| Software | Version | License | Provider |
|:---|:---|:---|:---|
| [Markdig](https://xoofx.github.io/markdig) | 1.0.0 | BSD 2-Clause | Alexandre Mutel |
| [Microsoft.Web.WebView2](https://aka.ms/webview) | 1.0.3800.47 | BSD 3-Clause | Microsoft Corporation |
| [Microsoft.Extensions.DependencyInjection](https://dot.net/) | 10.0.5 | MIT | Microsoft Corporation |
| [.NET runtime and libraries](https://dotnet.microsoft.com/) | 10.0 | MIT / .NET Library License | Microsoft Corporation |

---

## Markdig

Used to convert the user manual from Markdown to HTML.

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

Used to show Help in the app.

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

The WebView2 Runtime itself comes with Windows and isn't included in TwoTile.

---

## Microsoft.Extensions.DependencyInjection

Used to wire together the app's internal components (dependency injection).

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

## .NET runtime and libraries

TwoTile is built with .NET 10 and **includes the .NET runtime and libraries it needs to run** (self-contained). You don't need to install .NET separately.

The .NET source code is published under the MIT License, with the same text as Microsoft.Extensions.DependencyInjection above (`Copyright (c) .NET Foundation and Contributors`).

Redistribution of the included runtime is subject to the [.NET Library License](https://dotnet.microsoft.com/dotnet_library_license.htm). In line with it, §7 of the [Terms of Use](terms.en.md) includes terms that protect Microsoft and .NET. In summary:

- Microsoft makes **no warranties** about .NET and isn't liable for any damages.
- You won't reverse engineer, decompile, or disassemble .NET (except to the extent applicable law expressly permits it).
- If you redistribute TwoTile, **you must have recipients agree to terms that protect Microsoft and .NET at least as much.**

---

## About these notices

We update this document when TwoTile adds a package or moves to a new version of one. If you find anything missing or wrong, let us know through the [support contact](support.en.md).

For the terms of TwoTile itself, see the [Terms of Use](terms.en.md).

© 2026 poola-vii
