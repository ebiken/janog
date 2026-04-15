# Documentation Styles

## File Name and Directory Structure

- AsciiDoc files for Japanese documents MUST end with `*_ja.adoc`
- AsciiDoc files for English documents MUST end with `*_en.adoc`
- Each project has an index file named `index-<projectname>_[ja|en].adoc` which includes each chapter file under `chapters/`
- Images should be saved under `images/`
- Reference documents MUST be saved under `reference/`

Example directory structure:
```
<projectname>/
  index-<projectname>_ja.adoc
  index-<projectname>_en.adoc
  chapters/
    ch01_ja.adoc
    ch01_en.adoc
  images/
  reference/
```

## AsciiDoc Formatting Rules

- Always put one blank line before the first item of a list (lines starting with `* `, `. `, `** `, etc.) when it follows paragraph text or other non-list content.

Example:
```
Some paragraph text.

* First item
* Second item
```

## Diagram

- Use PlantUML for text based diagrams
- Use PNG format for image files 

## Math and Special Characters

Always use plain ASCII characters for math signs. Do not use Unicode math symbols.

| Instead of | Use  | Example |
|-----------|------|---------|
| × (U+00D7) | `x` or `*` | `2x H100`, `a * b` |
| − (U+2212) | `-` | `80 - 14` |
| – (U+2013) | `-` | `latency - 10` |
| ≈ (U+2248) | `~=` | `latency ~= 100ms` |
| ▼ | `v` | ASCII art arrows |
| √x (U+221A) | `sqrt(x)` | `sqrt(d_k)` |

Do not use these characters
- ▼
- × (multiplication sign U+00D7) — use `*` or `x` instead
- − (minus sign U+2212) — use `-` instead
- – (en dash U+2013) — use `-` instead
- ≈ — use `~=` instead
- √x (square root U+221A) — use `sqrt(x)` instead