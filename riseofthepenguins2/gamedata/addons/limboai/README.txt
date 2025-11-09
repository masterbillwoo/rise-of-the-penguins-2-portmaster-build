This folder is required for LimboAI GDExtension at runtime.

Place these files next to your game.pck under the same res:// paths:

- addons/limboai/limboai.gdextension  -> place into: gamedata/addons/limboai/
- addons/limboai/bin/limboai.gdextension -> some projects expect the descriptor here; if your log mentions res://addons/limboai/bin/limboai.gdextension, keep a copy in bin as well.
- addons/limboai/bin/liblimboai.linux.template_release.arm64.so -> place into: gamedata/addons/limboai/bin/

Notes:
- The filename must match exactly: liblimboai.linux.template_release.arm64.so
- Ensure it is the template_release build for Linux ARM64 (not the editor build).
- After copying, re-run the port and confirm the log no longer shows LimboAI extension errors.
