# Monkeyboard

A short description of what your project is A couple sentences on why you made the project

RP2040 SoC, USB-C connection port, 2 switches, crystal oscillator

# Photos

|Schematic|PCB|3D Render|
|---|---|---|
|![Schematic](https://github.com/emilyahmad/devboard/blob/main/PCB_DESIGN/images/devboard-schematic.png?raw=true)|![PCB](https://github.com/emilyahmad/devboard/blob/main/PCB_DESIGN/images/devboard-pcb.png?raw=true)|![3D](https://github.com/emilyahmad/devboard/blob/main/PCB_DESIGN/images/devboard-3dviewer.png?raw=true)|

# BOM

# BOM
| Item | Purpose | Quantity | Cost | Source |
|---|---|---|---|---|
| C1, C2 | 10uF decoupling capacitor | 2 | $0.0800 | JLCPCB Basic (CL10A106KP8NNNC) |
| C3, C18 | 1uF decoupling capacitor | 2 | $0.0660 | JLCPCB Extended (GRM155R60J105KE19D) |
| C4, C5, C19, C20, C22, C23, C24, C26 | 0.1uF decoupling capacitor | 8 | $0.0845 | JLCPCB Basic (CL05B104KO5NNNC) |
| C15, C16 | 33pF crystal load capacitor | 2 | $0.0130 | JLCPCB Basic (0402CG330J500NT) |
| C17, C21, C25 | 0.1uF decoupling capacitor | 3 | $0.0845 | JLCPCB Basic (CL05B104KO5NNNC) |
| J1 | USB-C receptacle | 1 | $0.9155 | JLCPCB Extended (TYPE-C-31-M-12) |
| J2, J3 | 20-pin GPIO header | 2 | — | Solder yourself |
| J4 | 3-pin SWD debug header | 1 | — | Solder yourself |
| R1, R2 | 5.1K CC pull-down resistor | 2 | $0.0090 | JLCPCB Basic (0402WGF5101TCE) |
| R3, R4 | 27Ω USB termination resistor | 2 | $0.0176 | JLCPCB Extended (0402WGF270JTCE) |
| R5, R7, R8 | 1K resistor | 3 | $0.0150 | JLCPCB Extended (RCT021KFLF) |
| R6 | 10K pull-up resistor | 1 | $0.0065 | JLCPCB Basic (0402WGF1002TCE) |
| SW1, SW2 | Push button | 2 | $0.5550 | JLCPCB Basic (TS-1088-AR02016) |
| U1 | MCP1700 3.3V LDO regulator | 1 | $2.4285 | JLCPCB Extended (MCP1700T-3302E/TT) |
| U2 | RP2040 microcontroller | 1 | $4.8810 | JLCPCB Extended (RP2040) |
| U3 | W25Q16 16Mbit flash memory | 1 | $6.3910 | JLCPCB Extended (W25Q16JVZPIQ TR) |
| Y1 | 12MHz crystal oscillator | 1 | $0.8382 | JLCPCB Extended (XJHCELNANF-12MHZ) |

Total: $16.38

<!--
reference
|RP2040|$0.94|https://www.lcsc.com/product-detail/C2040.html?s_z=s_p_RP2040&spm=wm.ssy.bg.0.xh&lcsc_vid=E1ENUAdXFlVdBAVSQFBZUQJQRFEMVgIFEgVcAgBRQgQxVlNRQFNbUVBfR1haUjsOAxUeFF5JWBYZEEoKFBINSQcJGk4%3D|
|Crystal oscillator|$0.07|https://www.lcsc.com/product-detail/C9002.html?s_z=s_q_CRYSTAL%252012MHZ&spm=wm.ssy.bg.0.xh&lcsc_vid=E1ENUAdXFlVdBAVSQFBZUQJQRFEMVgIFEgVcAgBRQgQxVlNRQFNbUVFTRlVXXzsOAxUeFF5JWBYZEEoKFBINSQcJGk4eFQsCAgIaSgADAwAHC0slRVFaV0oOAwwC|
|MCP1700 LDO, 3.3V|$0.98|https://www.lcsc.com/product-detail/C39051.html?s_z=n_q_mcp1700%2520tt&spm=wm.ssy.bg.16.xh&lcsc_vid=E1ENUAdXFlVdBAVSQFBZUQJQRFEMVgIFEgVcAgBRQgQxVlNRQFNbUVJRR1hcXjsOAxUeFF5JWBYZEEoKFBINSQcJGk4dAgUUFAk%3D|
|USB-C port, 16-pin|$0.08|https://www.lcsc.com/product-detail/C2988369.html?s_z=n_q_usb%2520c%252016&spm=wm.ssy.bg.0.xh&lcsc_vid=E1ENUAdXFlVdBAVSQFBZUQJQRFEMVgIFEgVcAgBRQgQxVlNRQFNbUVNSRVVYVzsOAxUeFF5JWBYZEEoKFBINSQcJGk4eFQsCAgIaSgADAwAHC0slRFheUlVIHxUDCw%3D%3D|
|W25Q128JVSIQ flash memory|$1.96|https://www.lcsc.com/product-detail/C97521.html?s_z=s_q_W25Q128JVSIQ&spm=wm.ssy.bg.0.xh&lcsc_vid=E1ENUAdXFlVdBAVSQFBZUQJQRFEMVgIFEgVcAgBRQgQxVlNRQFNbUVxWRFlWVTsOAxUeFF5JWBYZEEoKFBINSQcJGk4eFQsCAgIaSgADAwAHC0slRVhWX1dQTk8GEwkK|
|PCM5102A DAC|$1.02|https://www.lcsc.com/product-detail/C107671.html?s_z=n_q_pcm5102a&spm=wm.ssy.bg.1.xh&lcsc_vid=E1ENUAdXFlVdBAVSQFBZUQJQRFEMVgIFEgVcAgBRQgQxVlNRQFNbUV1XRVlaVjsOAxUeFF5JWBYZEEoKFBINSQcJGk4dAgUUFAk%3D|
|PAM8302AAD speaker amplifier|$0.21|https://www.lcsc.com/product-detail/C112137.html?s_z=n_q_pam8302aad&spm=wm.ssy.bg.0.xh&lcsc_vid=E1ENUAdXFlVdBAVSQFBZUQJQRFEMVgIFEgVcAgBRQgQxVlNRQFNbUV1SQFJbUzsOAxUeFF5JWBYZEEoKFBINSQcJGk4eFQsCAgIaSgADAwAHC0slRlFZUVNXWQkaCgg%3D|
|BQ25185 battery charging IC|$1.66|https://www.lcsc.com/product-detail/C19725033.html?s_z=s_p_BQ25185DLHR&spm=wm.ssy.bg.0.xh&lcsc_vid=E1ENUAdXFlVdBAVSQFBZUQJQRFEMVgIFEgVcAgBRQgQxVlNRQFNbUV1fQ1RWVzsOAxUeFF5JWBYZEEoKFBINSQcJGk4eFQsCAgIaSgADAwAHC0slRlBcVldRWQkaCgg%3D|
|SMD tactile switch, 6x6mm|$0.03|https://www.lcsc.com/product-detail/C49234152.html?s_z=n_q_5x5mm%2520button&spm=wm.ssy.bg.0.xh&lcsc_vid=RlQIVAdXEVQKUwJREwNdVlQAEQNaUAUCTlNbAgdURlMxVlNRQFJcUFFUTlhdUDsOAxUeFF5JWBYZEEoKFBINSQcJGk4%3D|
|Pin headers|$0.38|https://www.lcsc.com/product-detail/C2938459.html?s_z=h_q_pin%2520headers%252001x20&spm=wm.ssy.bg.1.xh&lcsc_vid=RlQIVAdXEVQKUwJREwNdVlQAEQNaUAUCTlNbAgdURlMxVlNRQFJcX1dVQFdZVTsOAxUeFF5JWBYZEEoKFBINSQcJGk4eFQsCAgIaSgADAwAHC0slRVhdX1BUQ08GEwkK|
|PCB|$0.42|https://cart.jlcpcb.com/quote?stencilLayer=2&stencilWidth=21&stencilLength=54&stencilCounts=5&plateType=1|
|Stencil|$3.05|https://cart.jlcpcb.com/quote?stencilLayer=2&stencilWidth=21&stencilLength=54&stencilCounts=5&plateType=1|

Total: $10.81 ($7.76 w/o stencil)

-->
# Notes

meow

