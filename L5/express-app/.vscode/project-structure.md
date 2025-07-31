# Project Structure

This file maintains an up-to-date list of project files and structure.

## File Structure

- 📁 `.vscode/`
  - 📄 `.vscode\project-structure.md` (Markdown)
- 📁 `controllers/`
  - 📄 `controllers\pizze.controller.js` (JavaScript)
    - *Imports:* `../services/pizze.service`
    - *Exports:* `module.exports`
- 📁 `middleware/`
  - 📄 `middleware\mainLogger.middleware.js` (JavaScript)
    - *Exports:* `module.exports`
  - 📄 `middleware\pizzaLogger.middleware.js` (JavaScript)
    - *Exports:* `module.exports`
  - 📄 `middleware\unavilabIeIds.middleware.js` (JavaScript)
    - *Exports:* `module.exports`
- 📁 `models/`
  - 📄 `models\Pizza.js` (JavaScript)
    - *Imports:* `mongoose`
    - *Exports:* `module.exports`
- 📁 `routes/`
  - 📄 `routes\pizze.route.js` (JavaScript)
    - *Imports:* `express`, `../controllers/pizze.controller`, `../middleware/pizzaLogger.middleware`
    - *Exports:* `module.exports`
- 📁 `services/`
  - 📄 `services\pizze.service.js` (JavaScript)
    - *Imports:* `../models/Pizza`
    - *Exports:* `module.exports`
- 📄 `db.js` (JavaScript)
  - *Imports:* `mongoose`
  - *Exports:* `module.exports`
- 📄 `index.js` (JavaScript)
  - *Imports:* `express`, `./db`, `./routes/pizze.route`, `./middleware/mainLogger.middleware`
- 📄 `package-lock.json` (JSON)
- 📄 `package.json` (JSON)

---
Last updated: 2025-07-31T16:08:17.647Z
