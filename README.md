Original Project : https://github.com/invoker-bot/LunaGC-Resources

# LunaGC Resources

An assembled resource dataset for LunaGC, centered on version 7.1 and supplemented with compatible data from other available resource snapshots. The collection brings together game configuration, scripts, scene data, text maps, and server-side mappings in one repository.

This is a community-maintained resource collection. It is not an official game release, a complete client dump, or a guarantee that every resource works with every LunaGC server build.

## Contents

| Directory | Contents |
| --- | --- |
| `BinOutput/` | Binary-exported ability and game configuration data |
| `ExcelBinOutput/` | Excel-exported game configuration tables |
| `Scripts/` | Lua scripts, including scene and quest logic |
| `ScriptSceneData/` | Scene script indexes and global scene metadata |
| `Server/` | Server-side mappings and supporting data |
| `TextMap/` | Localized text maps |

## Resource policy

- Keep the 7.1 value when the same stable record exists in multiple snapshots and its fields conflict.
- Add a record from another snapshot only when its stable key is absent and the records can be matched reliably. Do not merge tables by row number.
- Keep version-specific resources where their format or behavior differs. Lua API usage should follow the corresponding LunaGC server implementation where it is available.
- Treat this collection as best-effort and report unresolved conflicts or missing data instead of guessing.

These rules describe the intended curation approach; individual files can still contain upstream differences or incomplete data.

## Getting the files

Git LFS is used for the larger text-map, dialogue-table, and scene-index files. Install Git LFS before cloning so those files are checked out correctly:

```sh
git lfs install
git clone https://github.com/invoker-bot/LunaGC-Resources.git
```

If the repository was cloned without downloading LFS content, fetch it with:

```sh
git lfs pull
```

## Sources and credits

This collection builds on community resource work, including:

- [capyb2222/LunaGC-Resources](https://github.com/capyb2222/LunaGC-Resources) — 7.1 resource base
- [Merprose2/LunaGCR-Resources](https://github.com/Merprose2/LunaGCR-Resources) — 7.0 resource reference
- [kitkat033/LunaGC-Resources](https://github.com/kitkat033/LunaGC-Resources) — earlier resource base
- pmagixc, Meowereal, Hiro, Dimbreath, Yuuki, iam-akuzihs, Kuroo, IKunPS, and Rafs-kk for related resource contributions and inspiration

Please retain upstream attribution when reusing or redistributing files, and consult the source repositories for their own notices.

## License and attribution

No standalone license is provided for this collection. Game-derived data and upstream contributions remain subject to their respective rights and notices. This project is not affiliated with or endorsed by the game publisher.
