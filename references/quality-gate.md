# Delivery Quality Gate

Run the checks that apply to the current deliverables. If facts conflict, correct the evidence record first and then synchronize every affected artifact.

## Facts and Consistency

- The full software name, short name, version, and copyright-owner information match across all materials.
- Development and runtime environments are separate, and versions match dependency files, build files, or explicit user confirmation.
- Every listed function corresponds to source modules, menus, routes, controls, or authentic screenshots.
- Input formats, parameters, output fields, storage locations, and error messages match the actual software.
- Algorithm descriptions distinguish framework behavior, project configuration, training results, and original implementation.
- Dataset sizes, classes, splits, training parameters, and performance figures have direct evidence.
- Any database or external service is genuinely used by the software; tables, fields, and data flows are not invented.
- No names, applicants, hardware, class labels, or industry background from another software product remain.

## Document Structure

- Synchronized Chinese Markdown and DOCX files exist with the same filename stem, chapters, body text, tables, captions, and figure numbers.
- The DOCX uses portrait A4 pages with 25.4 mm top and bottom margins and 31.75 mm left and right margins.
- The cover sequence is exactly four empty paragraphs, full software name, version, one empty paragraph, the Chinese Design Specification label, four empty paragraphs, applicant line, and two empty paragraphs.
- The full name, version, and Design Specification label are centered and bold at 36 pt; the applicant line is centered and regular at 14 pt; the cover contains no date, logo, or decoration.
- The cover clearly identifies the software and version.
- The contents page uses a real updated automatic TOC. Both levels use regular 11 pt text and single-line spacing; level 1 has no left indent, level 2 has a 480-twip left indent, and both use a right-aligned 8296-twip tab with dot leaders connected to dynamic page numbers.
- Chapters 1 through 4 use the fixed Chinese titles for system overview, development environment, runtime environment, and implementation. Chapter 3 contains the fixed Sections 3.1 and 3.2.
- Chapter 1 contains only the Heading 1 `1.系统概述`, with no `1.x` subheading. Its body proceeds from background to problem, improved method, and evidence-supported effect, and the effect portion explicitly describes the complete software system.
- Section 3.1 contains the Chinese Table 1 caption and a 2-column, 5-row hardware table populated from the current project.
- Section 4.1 opens with the complete software workflow, and Figure 1 is the overall workflow diagram before any other figure.
- No chapter or section named `待完善信息` appears in the Markdown, DOCX body, or TOC; unresolved facts appear only in an external delivery note or audit list.
- Cover and contents headers are empty. The body header uses a left-aligned paragraph whose exact content order is `TAB → full software name plus version → TAB → dynamic PAGE field`, with center and right tab stops at 4153 and 8306 twips. The title is geometrically centered independently of the right-aligned page number; the header uses 9 pt sample-matched typography and a 0.75 pt bottom border, and body page numbering restarts at 1.
- Every footer is empty. The software name, version, and page number do not appear in a footer.
- Every figure and table is cited in the body; numbering and captions are continuous and consistent.
- Each operating procedure includes prerequisites, actions, and an observable result.
- There is no missing figure after a figure reference, control name that conflicts with a screenshot, or result description that conflicts with the displayed interface.
- A submission-ready document contains no TODO markers, unresolved placeholders, sample text, comments, or tracked changes.

## Source-Code Material

- Code comes from the registered version, and its source and ordering are recorded.
- It excludes third-party dependencies, caches, generated output, binaries, secrets, and personal data.
- Selected pages are consecutive, and page and line counts follow the currently verified applicable rule.
- The source-code material follows the requested header convention consistently; it does not move the software name or page number into a footer.
- Functions described in the manual can be traced to the selected code or the complete project.

## DOCX Visual Inspection

Use the DOCX renderer provided by the current environment and inspect every rendered page. Compare the cover, contents, body headings, hardware table, and body header against the fixed sample-derived layout. Confirm SimSun 12 pt body text, 1.5 line spacing, a two-character first-line indent, SimHei 14 pt Heading 1, and SimHei 12 pt Heading 2. Confirm the two TOC levels have the required 11 pt typography, indent, dot leader, and page number alignment. Confirm the body header begins with a real tab, centers the software name and version at the 4153-twip center tab independently of the page number, keeps the dynamic page number at the 8306-twip right tab, contains no leading spaces used for positioning, and uses the sample bottom border while every footer stays empty. Also confirm that text is not clipped or overlapping, required glyphs render correctly, images are legible, tables remain within the page, headings are not isolated at page bottoms, captions stay with their figures where practical, and the contents and page numbers display correctly.

If the renderer is unavailable, do not claim that visual inspection passed. State which structural checks were completed and which items still require a manual review in Microsoft Word.

## Delivery Note

Identify the files created or changed, the project version used as evidence, the major consistency issues resolved, and any facts still awaiting user confirmation. Keep internal audit notes outside the final submission document.
