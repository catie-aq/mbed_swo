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

To open a separated **GUI** to monitor SWO output via a J-Link probe, execute
`JLinkSWOViewer` with your device name, and CPU frequency e.g.:

```sh
JLinkSWOViewer -device STM32L496RG -cpufreq 80000000
```

To get the SWO output on a **command line interface**, the command is
* On Windows:
   ```sh
   JLinkSWOViewerCL -device STM32L496RG -cpufreq 80000000 -itmport 0
   ```
* On Linux:
   ```sh
   JLinkSWOViewer_CL -device STM32L496RG -cpufreq 80000000 -imtport 0
   ```
