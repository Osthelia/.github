# Osthelia Licenses

Every Osthelia project is published under one of the four licenses below. They all credit Osthelia as the author; they differ in what you are allowed to do with the code.

| License | File | Commercial use | Paid features | Advertising | Gambling | Hate speech | Other restrictions | Derivative works |
|---|---|---|---|---|---|---|---|---|
| **Osthelia Non-Commercial 2.0** | [NON-COMMERCIAL.md](NON-COMMERCIAL.md) | No | No | No | Forbidden | Forbidden | Scraping, scams, disinformation | Same license, source published |
| **Osthelia Limited Commercial 2.0** | [LIMITED-COMMERCIAL.md](LIMITED-COMMERCIAL.md) | Yes | No | Non-invasive only | Forbidden | Forbidden | No data resale | Same license, source published |
| **Osthelia Free 2.0** | [FREE.md](FREE.md) | Yes | Yes | Yes (no gambling ads) | Forbidden | Forbidden | — | Any license, restrictions passed on |
| **MIT** | [MIT.md](MIT.md) | Yes | Yes | Yes | Allowed | Allowed | — | Any license |

Attribution is required by all four licenses:

- **Osthelia licenses** — Copyright notice and file headers kept in the source, **plus** a visible notice for End-Users, as described in the project's Appendix A.
- **MIT** — Copyright notice kept in the source only. A visible credit can be *requested* in the project's README, but it cannot be required without leaving MIT.

The Osthelia License v1.0 is replaced by these licenses. Copies received under v1.0 stay under v1.0.

---

## Choosing a license

- **Non-Commercial** — Community tools, and anything that should never make money for someone else (our main platforms).
- **Limited Commercial** — Tools that companies or orgs may use, provided End-Users get everything for free and are not flooded with ads.
- **Free** — Building blocks we want to spread widely, while keeping them out of gambling and hate.
- **MIT** — Generic code with no esport-specific stakes (utilities, configs, templates), where adoption matters more than control.

---

## Applying a license to a project

### 1. `LICENSE.md`

Copy the chosen file to the root of the project as `LICENSE.md` and replace the placeholders:

| Placeholder | Example |
|---|---|
| `[YEAR]` | `2026` |
| `[PROJECT NAME]` | `GC-Stats-Website` |
| `[REPOSITORY URL]` | `https://github.com/Osthelia/GC-Stats-Website` |

### 2. Appendix A — project-specific attribution (Osthelia licenses)

The body of the license must stay identical across projects. **Only Appendix A changes**: it tells others how to credit *this* project. Replace the default rules with what fits the project, then remove the HTML comment. Always state:

- **The notice text** — Usually `Based on [Project](repo) by [Osthelia](https://osthelia.org/)`.
- **Where it is mandatory** — Footer, bot "About Me", link builder, CLI `--version`, package README…
- **Where it is not required** — If some output should stay clean (a stream overlay, an embed, a library's runtime), say so explicitly.

Examples:

- **Website / web app** — Keep the default rules (footer of every public page).
- **Discord bot** — Keep the default rules ("About Me").
- **Website next to an existing mention** — In the footer, where the original shows "Made by Osthelia". See [GC-Stats-Website](https://github.com/Osthelia/GC-Stats-Website/blob/main/LICENSE.md).
- **Website + bot in one repository** — One rule per Deployment type. See [GC-Scouting](https://github.com/Osthelia/GC-Scouting/blob/main/LICENSE.md).
- **Widget / overlay** — Not required on the rendered widget; mandatory in the software that generates or hands out the widget link.
- **Library / package** — Mandatory in the README or "credits" page of the product using it; not required at runtime.
- **Worker / API without UI** — Keep the default rules (the first service in the chain with a UI shows the notice), or name a specific page. See [RiotRelay](https://github.com/Osthelia/RiotRelay/blob/main/LICENSE.md) (legal pages).

### 3. `package.json`

```json
"license": "SEE LICENSE IN LICENSE.md"
```

For MIT, use `"license": "MIT"`.

### 4. Source file headers

```ts
/**
 * [PROJECT NAME] — [Short description of the file]
 *
 * @copyright Copyright (c) [YEAR] Osthelia — [PROJECT NAME]
 * @license   [REPOSITORY URL]/blob/main/LICENSE.md [LICENSE NAME]
 * @link      [REPOSITORY URL]
 */
```

`[LICENSE NAME]` is one of `Osthelia Non-Commercial License v2.0`, `Osthelia Limited Commercial License v2.0`, `Osthelia Free License v2.0` or `MIT`.

### 5. Project `README.md`

Add a **License** section that names the license and summarises how to credit the project:

```md
## License

[LICENSE NAME], see `LICENSE.md`. Source file headers must be kept, and any deployment must display
"Based on [PROJECT NAME] by Osthelia" as described in Appendix A of the license.
```

---

*Questions about a license, or a use it does not cover: [https://osthelia.org/](https://osthelia.org/).*
