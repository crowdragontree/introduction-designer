INTRODUCTION DESIGNER v1.0.3 - LOCAL BROWSER VERSION

Extract ZIP and open OPEN_Introduction_Designer.html in Chrome, Edge or Opera.

# Introduction Editor: Auto Make Room on Drop

Fixed the drag-and-drop overlap shown in the reported screenshots.

- **Auto make room is ON by default**, including when opening older saved drafts without this setting.
- **While dragging:** the selected item follows the pointer; no neighboring item moves.
- **On release:** the selected item stays where it was dropped; overlapping items are pushed downward, and any additional collisions are resolved in sequence. Unaffected items keep their exact positions. Side-by-side elements stay untouched.
- You can turn off Auto make room when you intentionally want layered elements to overlap. This does not affect Crop mode, which pans images within their crop frame.
- Supports drag from the element palette, existing layers, and on-canvas manipulation. All eight resize handles, alignment guides, divider image URLs, styled-border import, crop tools, and syntax-highlighted HTML remain available.
- Exact positions are preserved in reusable templates, autosaved drafts, the formatted Introduction HTML, and Studio's Save and Return flow. The 15,000-character check continues to use the full exported HTML.

### Verified
- Browser pointer-drag tests: collision-free motion until release, selected item preserved, collision cascades, opt-out overlap, autosave and formatted HTML export.
- Pure collision engine tests: cascading displacement, independent columns, unchanged untouched layers, safe failure at the maximum canvas height.
- Existing Introduction Designer, WebP Maker, and Blueprint Studio checks must still pass. Windows/Linux desktop executables require platform-native GitHub Actions build verification.

Templates and drafts are saved in local browser storage. Export to make a portable backup.
