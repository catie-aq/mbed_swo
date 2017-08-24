# Serial Wire Output (SWO) viewer for tracing purposes

- Example :
  
  ```
  #include "mbed.h"
  #include "swo.h"

  SWO_Channel SWO;

  int main() {
     SWO.printf("\r\nHello World from SWO\r\n");
  }
  ```
  
# JLink SWO Viewer
J-Link SWO Viewer is a tool which allows showing terminal output of the target performed via the SWO pin.

- In terminal : `JLinkSWOViewer`
