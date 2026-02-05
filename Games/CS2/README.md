# Counter-Strike 2 Configuration

Personal CS2 configuration files for optimized gameplay and performance.

## Files

### autoexec.cfg

Custom autoexec configuration that includes:

- **Keybinds**: Core movement, weapon slots, and mouse bindings
- **Buy Binds**: Numpad and F-key shortcuts for quick purchases
- **Mouse Settings**: Sensitivity (0.375), zoom ratio, and pitch/yaw values
- **Crosshair**: Cyan colored, small static crosshair (style 4)
- **Viewmodel**: Custom FOV (63) with adjusted offsets, left-handed
- **HUD**: Scaled HUD with radar tweaks
- **Sound**: Music disabled, voice chat configured
- **Network**: Max matchmaking ping set to 25
- **Performance**: Unlimited FPS, brightness at 2.6
- **Custom Aliases**: Damage display toggle, voice toggle, team equipment toggle
- **Advanced Grenade Binds**: Hold ALT + number keys for quick grenade selection

### launch_options.txt

Steam launch options for CS2:

```
+exec autoexec.cfg -nojoy -novid -high -freq 240 +cl_forcepreload 1 -threads 13 +violence_hblood 0 +fps_max 0 +mat_queue_mode 2 +engine_low_latency_sleep_after_client_tick true -allow_third_party_software
```

**Flags explained:**
- `+exec autoexec.cfg` - Execute autoexec on startup
- `-nojoy` - Disable joystick support
- `-novid` - Skip intro video
- `-high` - High CPU priority
- `-freq 240` - 240Hz refresh rate
- `+cl_forcepreload 1` - Preload assets
- `-threads 13` - CPU thread count
- `+violence_hblood 0` - Disable blood effects
- `+fps_max 0` - Unlimited FPS
- `+mat_queue_mode 2` - Multi-threaded rendering
- `+engine_low_latency_sleep_after_client_tick true` - Reduce input latency
- `-allow_third_party_software` - Allow overlays and third-party tools

## Installation

1. **autoexec.cfg**: Copy to `Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg\`
2. **Launch Options**: Right-click CS2 in Steam > Properties > Set Launch Options

## Notes

- Change `name "Change Me"` in autoexec.cfg to your preferred name
- Adjust `-threads` value based on your CPU
- Adjust `-freq` value to match your monitor's refresh rate
