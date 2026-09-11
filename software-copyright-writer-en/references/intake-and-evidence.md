# Intake and Evidence Record

Use this reference before drafting new registration documentation. Build the factual basis from the project first; do not ask the user to re-enter information that can be read from supplied artifacts.

## Inspect These Sources First

1. The project root, README files, launch scripts, and build files.
2. Dependency and version files such as `requirements.txt`, `pyproject.toml`, `package.json`, lockfiles, and container configuration.
3. Application entry points, business modules, UI files, routes, menus, button labels, and error messages.
4. Database migrations and schemas, model and training configuration, test records, and output examples.
5. Authentic screenshots, earlier manuals, application information, and templates supplied by the user.

Ignore virtual environments, dependency caches, build output, generated code, downloaded models, raw training data, and third-party source unless they directly affect runtime requirements or the user asks to include them.

## Evidence Fields

Record the applicable fields and retain a source path, screenshot, or explicit user confirmation for each one.

| Category | Fields |
|---|---|
| Identity | Full name, short name, version, copyright owner, development method, completion and publication information |
| Purpose | Intended users, application scenario, problem addressed, and product boundaries |
| Technology | Languages, frameworks, key dependencies, architecture, modules, algorithms, and rules |
| Environment | Verified operating systems, CPU, memory, GPU, external services, database, and launch method |
| Input and output | Input sources and formats, parameters, displayed results, exported files, and storage locations |
| Operation | Startup method, prerequisites, complete task flows, failures, and recovery behavior |
| Data | Data origin, schema, class labels, train-validation split, privacy, and licensing limits |
| Evidence | Source paths, configuration entries, UI text, authentic screenshots, logs, and test records |

## Evidence Strength

- Source code or configuration can directly support implemented behavior.
- Cross-check README files and older documentation against the current code. If versions conflict, use the code version selected by the user for this registration.
- A screenshot proves that an interface and visible result existed; it does not by itself prove a backend algorithm, performance claim, or data origin.
- A filename, comment, issue, or roadmap is a lead, not proof that a feature is implemented.
- Record which facts came from the user so that they are not later mistaken for conclusions derived from the code.

## Ask Only When Necessary

Analyze the artifacts and complete all supported sections before asking questions. Facts that normally require user confirmation include the copyright owner, method of acquiring the rights, completion date, first-publication status, and which code version corresponds to the filing when several versions are present.
