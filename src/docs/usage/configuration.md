# Configuration

Typ is configured through a single JSON file, `config.json`.

The configuration file must be present in a Typ project. See [Projects](./projects.md) for more information Project files.

## Configuration reference

### General options

| Option name | Description | Example |
| --- | --- | --- |
| `title` | The title of the book | `Alice in Wonderland` |
| `generateTableOfContents` | Whether to generate a table of contents based on headings | `true` |
| `pdfTkPath` | Path to the PDFtk executable. See [`installation`](./installation.md). | `C:\\Programs\\bin\\pdftk.exe` |

### Formatting options

These options control what the formatting of the book looks like.

These options generally have an equivalent CSS property. For instance, `textLineHeight` maps to [`line-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height), so could be set to `normal`, `2.5`, `3em`, and so on.

| Option name | Description | CSS | Example |
| --- | --- | --- | --- |
| `textLineHeight` | Sets the distance between lines of text | [`line-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height) | `2.5` |
| `pageMargin` | The margin between the edge of the page and the content | [`margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin) | `10px` |
| `pageSize` | The size of the page | [`size`](https://developer.mozilla.org/en-US/docs/Web/CSS/@page/size) | `A5`, `4in 6in` |
| `fontFamily` | Font for all text content | [`font-family`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-family) | `system-ui` |
| `fontSize` | Font size for main content | [`font-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size) | `2em` |

### Example `config.json`

```json
{
  "title": "Alice in Wonderland",
  "fontFamily": "Arial",
  "pageSize": "A5",
  "pageMargin": "70pt 60pt 70pt",
  "textLineHeight": "200%",
  "fontSize": "24pt",
  "generateTableOfContents": true,
  "pdfTkPath": "C:\\Programs\\bin\\pdftk.exe"
}
```