---
"emdash": patch
---

Preserve superscript and subscript marks in the in-page visual editor

`InlinePortableTextEditor` now registers TipTap's Superscript and Subscript mark extensions and maps the `superscript` and `subscript` Portable Text decorators through the ProseMirror round-trip. It also imports the existing mark-safety assertions, so loading or saving content with any remaining unsupported marks will throw instead of silently stripping them.
