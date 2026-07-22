# Submodules for AyuGram 7.0.4

Ayu-patched `lib_ui`, `lib_tl`, and `codegen` for tdesktop 7.0.4 are stored as branches on this repository:

| Submodule | Branch | Base (desktop-app) |
|-----------|--------|--------------------|
| Telegram/lib_tl | `submodule/lib_tl` | aa7791326d |
| Telegram/codegen | `submodule/codegen` | 1996c7c61e |
| Telegram/lib_ui | `submodule/lib_ui` | 7662467e98 |

`.gitmodules` points their URLs at `hzzmonetvn/AyuGramDesktop` so `git submodule update --init` can fetch the commits.

To publish as standalone repos later:

```bash
git clone --branch submodule/lib_ui https://github.com/hzzmonetvn/AyuGramDesktop.git lib_ui
# create empty hzzmonetvn/lib_ui, then:
cd lib_ui && git remote set-url origin git@github.com:hzzmonetvn/lib_ui.git && git push -u origin HEAD:master-ui
```
