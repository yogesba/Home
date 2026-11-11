# Setup instructions

1. Create or use a **public** GitHub repository named `yogesba` under user `yogesba`.
2. Place `README.md` in the repository root.
3. Place `snake.yml` at `.github/workflows/snake.yml`.
4. In repository **Settings → Actions → General → Workflow permissions**, enable **Read and write permissions** if organization policy allows it. The workflow requests `contents: write` explicitly, but repository policy can override this.
5. Open **Actions → Generate contribution snake → Run workflow**. After it succeeds, GitHub creates the `output` branch and the snake image appears in the README. A nightly schedule refreshes it.
6. The hand GIF, typing SVG, header/footer banners and statistics rely on third-party image services. If a service is offline or blocked, its image may not render; the rest of the README stays readable.

GitHub profile READMEs do not allow arbitrary JavaScript or CSS animation. Using externally hosted GIF/animated SVG images is the appropriate approach.

Note: The banner service provides a `fadeIn` query option; behavior depends on the banner rendering service. The header/footer waves themselves are decorative shapes, not continuously moving waves.
