# Windows API

*(Formerly Win32 API)*

### Links

 - [Windows API index](https://docs.microsoft.com/en-us/windows/win32/apiindex/windows-api-list) at Microsoft

### Page contents

 - [Using a function only if it exists](#using-a-function-only-if-it-exists)

### Using a function only if it exists

```cpp
#include <windows.h>

// SetThreadDescription is only available starting with Windows 10.
// The following code is safe to run on earlier versions of Windows.

typedef HRESULT(WINAPI *SetThreadDescFunc)(HANDLE hThread, PCWSTR desc);

void MySetThreadDescription(const wchar_t* desc)
{
    HMODULE hMod = GetModuleHandle(L"kernel32");

    if (hMod == NULL)
        return;

    SetThreadDescFunc SetThreadDesc = (SetThreadDescFunc)GetProcAddress(hMod, "SetThreadDescription");

    if (SetThreadDesc == NULL)
        return;

    SetThreadDesc(GetCurrentThread(), desc);
}
```
