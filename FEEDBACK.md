# How the app links here

The app (`frontend/src/components/About/FeedbackModal.js`) opens, in a new tab:

    https://github.com/widgemo/shaggysheets-feedback/issues/new?template=<bug|feature|question>.yml&title=<prefix>&diagnostics=<text>

- `template` is one of the three issue forms in `.github/ISSUE_TEMPLATE/`.
- `title` is a prefix (`Problem: `, `Idea: `, `Question: `) the person completes.
- `diagnostics` pre-fills the form field with the id `diagnostics` (each form has one). It is only sent when the person leaves
  "Include technical details" ticked.

If the repository is renamed, change `BRAND.feedbackRepo` in `frontend/src/config/brand.js`.
