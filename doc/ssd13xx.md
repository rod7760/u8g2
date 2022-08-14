| **Cmd code**           | **SSD1305**          | **SSD1306**         | **SSD1306b**           | **SSD1309**  | **SSD1312**              | **SSD1317**              | **SSD1320**          | **SSD1322**          | **SSD1325**     | **SSD1326**      | **SSD1327**          | **SSD1328**   | **SSD1329**    |
|------------------------|----------------------|---------------------|------------------------|--------------|--------------------------|--------------------------|----------------------|----------------------|-----------------|------------------|----------------------|---------------|----------------|
| **Max res**            | 132 x 64 x 4         | 128 x 64 x 1        | 128 x 64 x 1           | 128 x 64 x 1 | 128 x 64 x 1             | 128 x 96 x 1             | 160 x 160 x 4        | 480 x 128 x 4        | 128 x 80 x 4    | 256 x 32 x 4     | 128 x 128 x 4        | 128 x 128 x 4 | 128 x 128 x 4  |
| **Pages**              | 0..7                 | 0..7                | 0..7                   | -            | 0..7                     | 0..11                    | -                    | -                    | -               | -                | -                    | -             | -              |
| **Pwr on delay**       | -                    | "stable"            | "stable"               | -            | -                        | 20ms                     | 20ms                 | "stable"             | "stable"        | "stable"         | "stable"             | "stable"      | -              |
| **Init to Data delay** | -                    | 100ms               | 100ms                  | -            | 100ms                    | 100ms                    | 100ms                | 100ms                | 100ms           | 100ms            | 100ms                | 100ms         | -              |
| **0x00**               | enable greyscale tab | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x00-0x1f**          | set page addr        | set page addr       | set page addr          | -            | set page addr (0x0-0x17) | set page addr (0x0-0x17) | -                    | -                    | -               | -                | -                    | -             | -              |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x15**               | -                    | -                   | -                      | -            | -                        | -                        | set col              | set col              | set col         | set col          | set col              | -             | set col        |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x20**               | mem adr h/v/pg       | mem adr h/v/pg      | mem adr h/v/pg         | -            | mem adr h/v/pg           | mem adr h/v/pg           | mem adr mod          | mem adr mod          | -               | -                | -                    | -             | -              |
| **0x21**               | set col addr         | set col addr        | set col addr           | -            | set col addr             | set col addr             | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x22**               | set pg addr          | set pg addr         | set pg addr            | -            | set pg addr              | set pg addr              | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x23**               | -                    | -                   | set fade               | -            | -                        | -                        | -                    | -                    | graph acc opts  | -                | -                    | -             | -              |
| **0x24**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | draw rect       | -                | -                    | -             | -              |
| **0x25**               | -                    | -                   | -                      | -            | -                        | -                        | portrait en/dis      | -                    | copy rect       | -                | -                    | -             | -              |
| **0x26**               | hscroll R setup      | hscroll R setup     | hscroll R setup        | -            | -                        | -                        | -                    | -                    | hscroll setup   | hscroll setup    | scroll               | -             | -              |
| **0x27**               | hscroll L setup      | hscroll L setup     | hscroll L setup        | -            | -                        | -                        | -                    | -                    | -               | -                | scroll               | -             | -              |
| **0x28**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x29**               | vscroll&hscroll R    | vscroll&hscroll R   | vscroll&hscroll R      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x2a**               | vscroll&hscroll L    | vscroll&hscroll L   | vscroll&hscroll L      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x2b**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x2c**               | -                    | -                   | content scroll R       | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x2d**               | -                    | -                   | content scroll L       | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x2e**               | stop scroll          | stop hscroll        | stop hscroll           | -            | -                        | -                        | end move             | end move             | stop hscroll    | stop hscroll     | end move             | -             | -              |
| **0x2f**               | start scroll         | start hscroll       | start hscroll          | -            | -                        | -                        | start move           | start move           | start hscroll   | start hscroll    | start move           | -             | -              |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x5c**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | write ram            | -               | -                | -                    | -             | -              |
| **0x5d**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | read ram             | -               | -                | -                    | -             | -              |
| **0x40-0x7f**          | disp start ln (0-63) | disp start ln (0-63) | disp start ln (0-63)   | -            | disp start ln (0-63)     | disp start ln (0-63)     | -                    | -                    | -               | -                | -                    | -             | -              |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x75**               | -                    | -                   | -                      | -            | -                        | -                        | set row              | set row              | set row         | set row          | set row              | -             | set row        |
| **0x81**               | contrast             | contrast            | contrast               | -            | contrast                 | contrast                 | contrast             | contrast             | contrast        | contrast         | contrast             | -             | contrast       |
| **0x82**               | brightness           | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | 2nd precharge  |
| **0x84**               | -                    | -                   | -                      | -            | -                        | -                        | resume ram disp      | resume ram disp      | current (ND)    | ¼ current        | nop                  | -             | -              |
| **0x85**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | current (ND)    | ½ current        | nop                  | -             | -              |
| **0x86**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | current (ND)    | ¾ current (ND)   | nop                  | -             | -              |
| **0x87**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | current (ND)    | F current        | -                    | -             | -              |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x8d**               | -                    | charge pump (on/off) | charge pump (7.5V..9V) | -            | charge pump (7.5V..10V)  | -                        | charge pump 1?       | -                    | -               | -                | -                    | -             | -              |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0x90**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | icon ctl       |
| **0x91**               | set color tab        | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | icon current   |
| **0x92**               | color of bank1-16    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | icon current   |
| **0x93**               | color of bank32-63   | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | icon on/off    |
| **0x94**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | icon all       |
| **0x95**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | icon blink     |
| **0x96**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | icon duty      |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xa0**               | seg remap std        | seg remap std       | seg remap std          | -            | -                        | seg remap std            | remap                | remap & dual         | remap           | remap            | remap                | -             | remap          |
| **0xa1**               | seg remap inv        | seg remap inv       | seg remap inv          | -            | -                        | seg remap inv            | start line           | start line           | start line      | start line       | start line           | -             | start line     |
| **0xa2**               | -                    | -                   | -                      | -            | -                        | disp start ln (0-95)     | offset               | offset               | offset          | offset           | offset               | -             | offset         |
| **0xa3**               | vscroll area         | vscroll area        | vscroll area           | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xa4**               | disp ram             | disp ram            | disp ram               | -            | disp ram                 | disp ram                 | disp mode            | norm disp            | norm disp       | norm disp        | mode                 | -             | mode           |
| **0xa5**               | disp all px ON       | disp all px ON      | disp all px ON         | -            | disp all px ON           | disp all px ON           | -                    | disp all px ON       | disp all px ON  | disp all px ON   | -                    | -             | -              |
| **0xa6**               | norm disp            | norm disp           | norm disp              | -            | norm disp                | norm disp                | norm disp            | disp all px OFF      | disp all px OFF | disp all px OFF  | -                    | -             | -              |
| **0xa7**               | inverse disp         | inverse disp        | inverse disp           | -            | inverse disp             | inverse disp             | -                    | inverse disp         | inverse disp    | inverse disp     | mode                 | -             | mode           |
| **0xa8**               | mux ratio 16..64     | mux ratio 16..64    | mux ratio 16..64       | -            | mux ratio 16..64         | mux ratio 16..64         | mux ratio            | enter partial mode   | mux ratio       | mux ratio 16..32 | mux ratio            | -             | mux ratio      |
| **0xa9**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | exit partial mode    | -               | -                | -                    | -             | -              |
| **0xaa**               | resv                 | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xab**               | dim mode             | -                   | -                      | -            | -                        | -                        | -                    | config vcc           | -               | -                | regulator            | -             | -              |
| **0xac**               | disp on (dim)        | -                   | -                      | -            | -                        | -                        | charge pump 2?       | -                    | -               | -                | -                    | -             | -              |
| **0xad**               | config vcc           | -                   | select Iref            | -            | select Iref              | select Iref              | select Iref          | -                    | master config   | -                | -                    | -             | -              |
| **0xae**               | disp on (bright)     | disp on             | disp on                | -            | disp on                  | disp on                  | disp on              | sleep on             | disp on         | disp on          | disp on              | -             | disp on        |
| **0xaf**               | disp off             | disp off            | disp off               | -            | disp off                 | disp off                 | disp off             | sleep off            | disp off        | disp off         | disp off             | -             | disp off       |
| **0xb0**               | set pg addr 0        | set pg addr 0       | set pg addr 0          | -            | set pg addr 0            | set pg addr 0            | -                    | -                    | comp enable     | -                | -                    | -             | -              |
| **0xb1**               | set pg addr 1        | set pg addr 1       | set pg addr 1          | -            | set pg addr 1            | set pg addr 1            | phase len            | phase len            | phase len       | phase len        | phase len            | -             | phase len      |
| **0xb2**               | set pg addr 2        | set pg addr 2       | set pg addr 2          | -            | set pg addr 2            | set pg addr 2            | frame freq           | -                    | row period      | frame freq       | nop                  | -             | frame freq     |
| **0xb3**               | set pg addr 3        | set pg addr 3       | set pg addr 3          | -            | set pg addr 3            | set pg addr 3            | clock div [2]        | clock div [2]        | div ratio [3]   | clock div [2]    | clock div            | -             | clock div [2]  |
| **0xb4**               | set pg addr 4        | set pg addr 4       | set pg addr 4          | -            | set pg addr 4            | set pg addr 4            | -                    | -                    | comp level      | -                | -                    | -             | -              |
| **0xb5**               | set pg addr 5        | set pg addr 5       | set pg addr 5          | -            | set pg addr 5            | set pg addr 5            | -                    | GPIO                 | -               | -                | GPIO                 | -             | -              |
| **0xb6**               | set pg addr 6        | set pg addr 6       | set pg addr 6          | -            | set pg addr 6            | set pg addr 6            | -                    | 2nd phase            | -               | -                | 2nd phase            | -             | -              |
| **0xb7**               | set pg addr 7        | set pg addr 7       | set pg addr 7          | -            | set pg addr 7            | set pg addr 7            | -                    | -                    | -               | default gray     | -                    | -             | default gray   |
| **0xb8**               | -                    | -                   | -                      | -            | -                        | set pg addr 8            | gray level           | gray scale tab       | gray scale tab  | gray scale tab   | gray scale tab       | -             | gray level     |
| **0xb9**               | -                    | -                   | -                      | -            | -                        | set pg addr 9            | -                    | set linear greyscale | -               | -                | set linear greyscale | -             | -              |
| **0xba**               | -                    | -                   | -                      | -            | -                        | set pg addr 10           | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xbb**               | -                    | -                   | -                      | -            | -                        | set pg addr 11           | -                    | precharge volt       | -               | 2nd precharge    | nop                  | -             | 2nd charge     |
| **0xbc**               | -                    | -                   | -                      | -            | -                        | -                        | precharge volt       | -                    | precharge volt  | precharge volt   | precharge volt       | -             | precharge volt |
| **0xbd**               | -                    | -                   | -                      | -            | -                        | -                        | set vp?              | -                    | -               | -                | -                    | -             | -              |
| **0xbe**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | comh volt            | comh volt       | comh volt        | comh volt            | -             | comh volt      |
| **0xbf**               | -                    | -                   | -                      | -            | -                        | -                        | greyscale gamma      | greyscale gamma      | VSL             | -                | -                    | -             | -              |
| **0xc0**               | com remap disab      | com remap disab     | com remap disab        | -            | com remap disab          | com remap disab          | com remap disab      | -                    | -               | -                | -                    | -             | -              |
| **0xc1**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | contrast current     | -               | -                | -                    | -             | -              |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xc7**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | master contrast      | -               | -                | -                    | -             | -              |
| **0xc8**               | com remap enab       | com remap enab      | com remap enab         | -            | com remap enab           | com remap enab           | com remap enab       | -                    | -               | -                | -                    | -             | -              |
| **0xc9**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xca**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | mux ratio (16-128)   | -               | -                | -                    | -             | -              |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xd3**               | disp offset          | disp offset         | disp offset            | -            | disp offset              | disp offset              | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xd4**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xd5**               | clock div ratio      | clock div ratio     | clock div ratio        | -            | clock div ratio          | clock div ratio          | -                    | -                    | -               | -                | fn select B          | -             | -              |
| **0xd6**               | -                    | -                   | disp zoom-in           | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xd7**               | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xd8**               | area color mode      | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xd9**               | precharge period     | precharge period    | precharge period       | -            | precharge period         | precharge period         | dischg/prechg period | -                    | -               | -                | -                    | -             |
| **0xda**               | set com config       | set com config      | set com config         | -            | set com config           | set com config           | seg pin conf         | -                    | -               | -                | -                    | -             |
| **0xdb**               | set vcomh            | set vcomh           | set vcomh              | -            | set vcomh                | set vcomh                | set vcomh            | -                    | -               | -                | -                    | -             |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xe0**               | enter RmW mode       | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xe3**               | nop                  | nop                 | nop                    | -            | nop                      | nop                      | -                    | -                    | nop             | -                | -                    | -             | nop            |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xee**               | exit RmW mode        | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |
| **0xfd**               | -                    | -                   | -                      | -            | cmd lock                 | cmd lock                 | -                    | cmd lock             | -               | cmd lock         | cmd lock             | -             | cmd lock       |
| **..**                 | -                    | -                   | -                      | -            | -                        | -                        | -                    | -                    | -               | -                | -                    | -             | -              |