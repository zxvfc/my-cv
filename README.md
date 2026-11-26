# Valentin Isipchuk — Full-stack Developer

[![Deploy](https://github.com/zxvfc/my-cv/actions/workflows/deploy.yml/badge.svg)](https://github.com/zxvfc/my-cv/actions/workflows/deploy.yml)

Full-stack developer with 8+ years of experience in Java, Kotlin, Go, TypeScript and PHP across fintech, Web3 and cloud platforms. I build AI-native development workflows with Claude Code, Codex and OpenCode.

## View the CV

|            | English | Русский |
|------------|---------|---------|
| **Online** | [View online](https://zxvfc.github.io/my-cv/?lang=en) | [Открыть онлайн](https://zxvfc.github.io/my-cv/?lang=ru) |
| **PDF**    | [Download PDF](https://zxvfc.github.io/my-cv/cv-isipchuk.pdf) | [Скачать PDF](https://zxvfc.github.io/my-cv/cv-isipchuk-ru.pdf) |

## Contacts

- Email: [velya.96@gmail.com](mailto:velya.96@gmail.com)
- Telegram: [t.me/zxvfc](https://t.me/zxvfc)
- LinkedIn: [linkedin.com/in/va-is](https://linkedin.com/in/va-is)
- Location: Bangkok, Thailand (open to remote work)

## How it works

The whole CV is one file, [`index.html`](index.html), with no build tools or dependencies.

- **Two languages in one page.** Every text has an English and a Russian version (`lang="en"` / `lang="ru"`), and CSS shows only the selected one. Pick the language with the EN/RU buttons or the `?lang=` URL parameter; the choice is remembered in the browser.
- **Print-ready.** A4 print styles keep each language version on one page.
- **Automatic PDFs and deploy.** On every push to `main`, the [deploy workflow](.github/workflows/deploy.yml) prints both versions to PDF with headless Chrome, checks they were created, and publishes the page and PDFs to GitHub Pages.

## Editing

1. Edit `index.html`. When you change a text, update both the `lang="en"` and `lang="ru"` versions.
2. Open the file in a browser to preview it, and switch between EN and RU.
3. Check that each version still fits on one page: open the print preview (Ctrl/Cmd + P), or generate the PDFs locally:

   ```sh
   google-chrome --headless --no-pdf-header-footer --print-to-pdf=cv-en.pdf "file://$PWD/index.html?lang=en"
   google-chrome --headless --no-pdf-header-footer --print-to-pdf=cv-ru.pdf "file://$PWD/index.html?lang=ru"
   ```

4. Push to `main`. The site and PDFs update in a minute or two.
