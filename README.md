# Serial Wire Output (SWO) Library

Usage:
  
```cpp
#include "mbed.h"
#include "swo.h"

using namespace sixtron;

static SWO swo;

int main() {
   swo.printf("Hello, World!\n");
}
```
  
To monitor SWO output via J-Link debug and trace probe, execute
`JLinkSWOViewer` with your device name, and CPU frequency e.g.:

```sh
JLinkSWOViewer -device STM32L496RG -cpufreq 80000000
```
