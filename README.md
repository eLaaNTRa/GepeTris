# 🎮 GePetris

A retro-styled Tetris built in a single HTML file by ChatGPT & Gemini 2.5 Pro (Canvas + JS).  
Supports **Keyboard + Mouse + Controller** (Works with standard gamepads).  
Includes ghost piece, DAS, wall kicks, banners, SFX, and controller vibration.


## 🎮 Controls

### Keyboard
- **← / →** Move (DAS)  
- **↓** Soft drop  
- **Space** Hard drop  
- **Z / X** Rotate CCW / CW  
- **C** Hold  
- **P** Pause  
- **Enter** Restart

### Mouse
- **Left click (center third)** Rotate CW  
- **Left click (left/right thirds)** Move left/right  
- **Right click** Hold (context menu disabled on canvas)  
- **Double-click** Hard drop  
- **Wheel Up/Down** Rotate CW/CCW

### Controller (Standard mapping)
- **D-Pad** Move / Soft drop  
- **A (0)** Rotate CW  
- **B (1)** Rotate CCW  
- **Y (3)** Hold  
- **X (2)** Hard drop  
- **Select (8)** Pause  
- **Start (9)** Restart / Unpause  
- **Vibration**: triggers on a **Tetris** (4-line clear) if supported

> If your controller doesn’t vibrate, the browser/driver may not expose `vibrationActuator`.

## 🔊 Audio
- Short **tick** sound on horizontal moves only  
- Progressive tones on line clears:
  - 1 line → tone 1  
  - 2 lines → 2-note chime  
  - 3 lines → 3-note run + “Triple Clear!” banner  
  - 4 lines → **“Boom! Tetris!”** + bassy boom + controller rumble  

> Audio starts after your first interaction (browser autoplay policy).

## ⚙️ Rotation Mode
UI button: **Up = CCW/CW (switch)** toggles the Up-arrow behavior.  
(Z = CCW, X = CW always.)

## 🧠 Features
- Smooth DAS with independent left/right timing  
- SRS-style wall-kick attempts near borders  
- Ghost piece rendered below active piece  
- Hold with once-per-drop rule; resets on game over  
- Subtle single/double clear flash; triple banner; **Boom! Tetris!** banner  
- Speed ramps gently with score, starting a bit faster than default  
- LocalStorage high score  
- Retro **Press Start 2P** styling  
- “Vibe-Coded by: **Pranav Kulkarni aka eLaNTRa**”

## 🐛 Troubleshooting
- **No sound?** Click the page or press any key once (autoplay unlock).  
- **No vibration?** Not all browsers/controllers expose haptics. Brave usually does on desktop with supported pads.  
- **Controller not detected?** Press a controller button to wake it, or reconnect via USB/Bluetooth.

Enjoy!
