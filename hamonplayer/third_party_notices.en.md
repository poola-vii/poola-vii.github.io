---
layout: page
title: Third-Party Notices
lang: en
---

**Applies to: HamonPlayer 1.0.6 (Windows version; Microsoft Store version and setup.exe version)**

HamonPlayer includes the following third-party software. Each is subject to the terms set by its provider. The notices each license requires are below.

- **NAudio.Core, NAudio.Wasapi** — Version: 2.2.1 / License: MIT / Provider: Mark Heath / https://github.com/naudio/NAudio
- **Vortice.MediaFoundation, Vortice.DirectX** — Version: 3.8.3 / License: MIT / Provider: Amer Koleci and Contributors / https://github.com/amerkoleci/Vortice.Windows
- **Vortice.Mathematics** — Version: 2.1.0 / License: MIT / Provider: Amer Koleci and Contributors / https://github.com/amerkoleci/Vortice.Mathematics
- **SharpGen.Runtime, SharpGen.Runtime.COM** — Version: 2.4.2-beta / License: MIT / Provider: Alexandre Mutel, Jeremy Koritzinsky, Amer Koleci / https://github.com/SharpGenTools/SharpGenTools
- **.NET runtime and libraries** — Version: 10.0 / License: MIT, .NET Library License / Provider: Microsoft Corporation / https://dotnet.microsoft.com/
- **Windows SDK components for .NET (Microsoft.Windows.SDK.NET, WinRT.Runtime)** — Version: 10.0.19041.57 / License: Microsoft Windows SDK license terms / Provider: Microsoft Corporation / https://aka.ms/WinSDKLicenseURL
- **Inno Setup** (only in the installer and uninstaller of the setup.exe version) — Version: 6.6.1 / License: Inno Setup License / Provider: Jordan Russell, Martijn Laan / https://jrsoftware.org/

The Windows version of HamonPlayer doesn't use any other packages (external libraries). We'll add the software included in the phone version (Android) when the phone version is released.

---

## NAudio.Core, NAudio.Wasapi

Used to check whether other apps are playing sound (so that HamonPlayer can pause when another app plays sound).

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

## Vortice.MediaFoundation, Vortice.DirectX, Vortice.Mathematics

Used with Media Foundation (the playback system in Windows) to play songs, show videos, and measure the loudness of songs.

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

## SharpGen.Runtime, SharpGen.Runtime.COM

Used by Vortice (above) to call Windows components.

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

## .NET runtime and libraries

HamonPlayer is built with .NET 10 and **includes the .NET runtime and libraries it needs to run** (self-contained). You don't need to install .NET separately.

The .NET source code is published under the following MIT License.

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

Redistribution of the included runtime is subject to the .NET Library License (https://dotnet.microsoft.com/dotnet_library_license.htm). Accordingly, §7 of the Terms of Use contains provisions that protect Microsoft and .NET. In summary:

- Microsoft **makes no warranties** for .NET and isn't liable for any damages.
- You won't reverse engineer, decompile, or disassemble .NET, except to the extent that applicable law expressly permits it.
- If you redistribute HamonPlayer, **you must have recipients agree to terms that protect Microsoft and .NET at least as much.**

---

## Windows SDK components for .NET (Microsoft.Windows.SDK.NET, WinRT.Runtime)

Used to call Windows components: to show the current song's name and album art in the Windows media controls and receive the media keys on your keyboard, to read song tags, and, in the Microsoft Store version, to turn starting with Windows on or off.

These components are on Microsoft's redistribution list ("Windows SDK redist lists", https://learn.microsoft.com/en-us/legal/windows-sdk/redist, under "Microsoft.Windows.SDK.NET.Ref"). They are distributed unmodified as part of the app, so that it can call Windows APIs. Redistribution of these components is subject to the Microsoft Windows SDK license terms ("MICROSOFT SOFTWARE LICENSE TERMS — MICROSOFT WINDOWS SOFTWARE DEVELOPMENT KIT (SDK) FOR WINDOWS 10", https://aka.ms/WinSDKLicenseURL). These terms require that recipients agree to terms that protect the components at least as much. Accordingly, §7 of the Terms of Use contains provisions that protect Microsoft and these components.

---

## Inno Setup

Used for the installer and uninstaller of the setup.exe version. It isn't included in the Microsoft Store version.

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

## About these notices

We'll update this document when HamonPlayer starts using more software or updates the versions it uses. If you notice anything missing or wrong, let us know through the support contact (https://github.com/poola-vii/support).

© 2026 poola-vii
