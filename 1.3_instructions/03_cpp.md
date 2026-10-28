

## 🧱 Checkpoint 4 — C++ Program (commit: `cpp-basic`)
**Files**: `cpp/main.cpp`

```cpp
#include <iostream>
using namespace std;
int main() {
    int x = 5;
    int y = x + 3;
    cout << "Result: " << y << endl;
    return 0;
}
```
Compile, run, and inspect:
```bash
g++ main.cpp -o main
./main
objdump -d main | head -n 60 > main_cpp.disasm.head.txt
```
**Prompts (add to `journal/04_cpp.md`)**:
- Screenshot with the program output.
- <img width="560" height="533" alt="Screenshot 2026-10-28 194553" src="https://github.com/user-attachments/assets/b82d030a-b357-430d-bb2a-8b139a4d2048" />
- Compared to C, how does the binary size and disassembly differ (at a glance)? Why might this be?

- Compared to C, the C++ program may have a larger binary size and more disassembly instructions. This is because C++ uses iostream and cout for output, which can require additional library code compared to C's printf. The disassembly may also look more complex because the compiler generates extra instructions to handle C++ features. Both programs calculate the result as 8, but their compiled machine code can be different.
