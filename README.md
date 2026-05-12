# Framebuffer-connector-type-Hex-value-Connection-type-Associated-monitor

 % for i in {0..5}; do          
  echo "=== Framebuffer @${i} ==="
  ioreg -r -n "ATY,AMD,RadeonFramebuffer@${i}" -l | grep -E "connector-type|port-number|IODisplayName|display0|name"
  echo ""

<img width="657" height="242" alt="Captura de pantalla 2026-05-12 a las 11 21 19" src="https://github.com/user-attachments/assets/1d0cf947-e16c-4883-b414-6e34a6eb6d72" />

<img width="575" height="756" alt="Captura de pantalla 2026-05-12 a las 11 25 26" src="https://github.com/user-attachments/assets/f0d23e17-2b04-4d0a-a056-b18471d9dc84" />

Let's analyze the command to find out the necessary data:

=== Framebuffer @2 ===

"connector-type" = 1024

AppleDisplay-220e-3545"


=== Framebuffer @3 ===

"connector-type" = 2048

AppleDisplay-22f0-3320"

@1 220e-3545 HP 24fw

2048 Sets the port to DisplayPort(<00 08 00 00>)

<img width="471" height="243" alt="Captura de pantalla 2026-05-12 a las 11 49 50" src="https://github.com/user-attachments/assets/2a7ba34a-841d-479e-b784-a8fc00c47a08" />


@2 22f0-3320 HP 24es

1024 Sets the port to HDMI<00 04 00 00>)

<img width="471" height="243" alt="Captura de pantalla 2026-05-12 a las 11 49 50" src="https://github.com/user-attachments/assets/d684b773-8fd1-489e-984b-4c9027c449d4" />





