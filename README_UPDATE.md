# Altera Update Repository Layout

Recommended GitHub layout:

```text
resource_manifest.json
module_manifest.json
resources/
  clause_lib.json
  seo_category_keywords.json
  ui_theme.qss
  ui_config.json
GitHub Releases
  altera_V8.1.exe
  core_logic.pyd
  seo_engine.pyd
  excel_engine.pyd
```

Update levels:

- Resource update: edit files under `resources/`, then update `resource_manifest.json`.
- Core module update: compile `.py` to `.pyd`, upload `.pyd` files to a GitHub Release, then update `module_manifest.json`.
- Full app update: upload a new `.exe` to a GitHub Release.

Keep source code in a private repository. Put only compiled `.exe` / `.pyd` files and safe resource files in this public update repository.
