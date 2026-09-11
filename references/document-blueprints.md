# Document Blueprints

Use the fixed layout and first-four-chapter structure in this file for every new Chinese software copyright manual. Software type changes only the detailed Chapter 4 subsections and the chapters after Chapter 4.

## Required Output Pair

Create synchronized Chinese Markdown and Word DOCX files. Finish the Markdown first, then generate the DOCX from the same content. Use the same filename stem. Keep chapters, body text, tables, captions, and figure numbers synchronized; use DOCX to implement the cover, automatic contents, pagination, typography, and image layout.

## Fixed Page and Typography Rules

- Use portrait A4 pages, 210 mm by 297 mm.
- Set top and bottom margins to 25.4 mm and left and right margins to 31.75 mm.
- Use SimSun 12 pt for Chinese body text and Times New Roman 12 pt for Latin text and numbers. Justify the body, use 1.5 line spacing, and indent the first line by two Chinese characters.
- Use SimHei 14 pt in black for Heading 1 and SimHei 12 pt in black for Heading 2. Do not insert a tab between a heading number and its title.
- Use centered, bold, 9 pt captions with SimSun for Chinese and Times New Roman for Latin text. Keep caption placement consistent for each figure and table type.
- Do not add colored headings, decorative rules, icons, logos, a date, or extra cover metadata.

## Fixed Cover

Use this exact paragraph sequence and add no other cover content:

1. Four empty body paragraphs at the top.
2. The full software name in its own centered paragraph, bold 36 pt, using SimSun for Chinese and Times New Roman for Latin text and numbers. Do not reduce the font for a long title; allow natural wrapping.
3. The next paragraph contains `V1.0` or the verified version, centered, bold Times New Roman 36 pt.
4. One empty paragraph.
5. The next paragraph contains the Chinese text for "Design Specification," centered, bold SimSun 36 pt.
6. Four empty body paragraphs.
7. The next paragraph uses the Chinese applicant label followed by an ASCII colon, two spaces, and the applicant name. Center it in regular 14 pt, using SimSun for Chinese and Times New Roman for Latin text and numbers.
8. Two empty paragraphs, then a page or section break before the contents.

Do not place a date, address, contact details, slogan, copyright notice, logo, or decorative element on the cover. An unresolved applicant may be marked in a working draft but never in a submission-ready file.

## Contents and Fixed Chapters

Place the contents on a separate page after the cover. Its Chinese title is `目 录` in SimHei 18 pt, bold and centered. Build the entries with a real automatic TOC field covering Heading 1 and Heading 2; do not type periods or page numbers manually. Update all fields after pagination is final.

Match the sample TOC formatting:

- Use SimSun 11 pt for Chinese and Times New Roman 11 pt for Latin text and numbers at both TOC levels. Use black, regular text and single-line spacing.
- TOC level 1 has no left or first-line indent.
- TOC level 2 has a 480-twip left indent, approximately 0.85 cm, and no first-line indent.
- At both levels, set a right-aligned tab stop at 8296 twips with a dot leader so the visible `...` runs continuously from the title to the dynamic page number.
- Include only actual numbered Heading 1 and Heading 2 paragraphs. The entry wording, numbering, indentation, leader dots, and page numbers must match the body after the TOC field is updated.

Use these exact Chinese chapter titles for the first four chapters and first two Chapter 3 subsections:

1. `1.系统概述`
2. `2.软件开发环境`
3. `3.软件运行环境`
   - `3.1硬件环境要求`
   - `3.2软件环境配置`
4. `4.软件实现方法`

Chapter 1 consists of the single Heading 1 `1.系统概述` followed directly by coherent body paragraphs. Do not create `1.1`, `1.2`, or any other subordinate heading. Develop the narrative in this order: application background, the specific problem arising in that setting, the improved method introduced to solve the problem, and the evidence-supported effect achieved by that method. In the effect portion, explicitly describe the complete software system and how its input, core processing, and output work together. Avoid unsupported performance figures or generic claims. Chapter 2 lists the development language, platform, tools, and main libraries in Chinese `(1)`, `(2)`, `(3)` sequence, using only verified facts.

Section 3.1 begins with a paragraph describing verified runtime hardware and referring to Table 1. Place the Chinese caption meaning "Table 1 Hardware Configuration Requirements" above an unshaded black single-line grid. Use a fixed 2-column, 5-row table. The headers mean "Hardware Configuration Requirement" and "Parameter Requirement"; the remaining rows are GPU, CPU, memory, and storage. If no discrete GPU is required, state that instead of copying a sample model. Use an overall width of about 15.99 cm, column widths of about 7.52 cm and 8.48 cm, the Word Table Grid style, SimSun 12 pt body text, and 1.5 line spacing.

Section 3.2 begins with a Chinese sentence introducing the required software environment, followed by one dependency per line in Chinese `(1)`, `(2)`, `(3)` format. Include only verified operating systems, runtimes, frameworks, databases, and other dependencies.

Chapter 4 subsection titles and count depend on the project. Section 4.1 must begin by explaining the complete software process and must place the document's first figure, a Chinese-captioned overall software workflow, before every architecture, interface, or result figure. Refer to Figure 1 in the body before inserting it. The flowchart must cover startup or input, required configuration, core processing, major decision branches, result display or saving, and completion, with every node supported by source code or authentic operation evidence.

Organize Chapter 5 and later chapters around verified functions and operations, data or databases, result saving, and error handling as applicable. Never append a Chapter 7 or any other numbered chapter or section named `待完善信息`. Put unresolved facts only in the external delivery note or audit list, never in the Markdown or DOCX submission body or its TOC.

## Header, Footer, and Page Number

Use section breaks so the cover, contents, and body can have different headers. Keep the cover and contents headers empty. Keep all footers empty; the software name and page number must never appear in a footer.

Starting on the first body page, use one header paragraph that matches the sample:

- Put the full registered software name immediately followed by the verified version at the geometric center of the usable page width, for example `软件全称V1.0`. Use SimSun 9 pt for Chinese and Times New Roman 9 pt for Latin text and numbers.
- Use one left-aligned header paragraph with a center tab stop at 4153 twips and a right tab stop at 8306 twips. Its content sequence must be: a tab character, the software name plus version, a second tab character, and a real `PAGE` field. Do not place the title before the first tab, do not center the whole paragraph, and do not use spaces to imitate centering.
- The first tab anchors the title independently at the center tab stop; the second tab anchors the PAGE field at the far-right tab stop. This prevents the page number from shifting the title away from the page center. Do not type a fixed page number.
- Add a black single bottom border of 0.75 pt to the header paragraph.
- Restart Arabic page numbering at `1` in the body section. Use a header distance of about 851 twips, approximately 15 mm, matching the sample.
- After generating the DOCX, update the PAGE fields and verify geometrically that the midpoint of the software-name text aligns with the center of the usable page width while the page number remains at the far right. If the verified registered name is too long to fit without colliding with the page number, allow it to wrap; do not abbreviate it and never compensate with leading spaces.

## Computer Vision and Machine Learning Software

A useful processing sequence is input source, preprocessing, model loading, inference, post-processing, visualization, and saving. Include dataset composition, annotation classes, splits, augmentation, training parameters, or deployment formats only when direct evidence is available.

Distinguish among:

- Capabilities supplied by a general model or framework.
- Capabilities produced by project configuration and training.
- Modules, rules, or architecture changes implemented by the project.

Separate image, video, and camera workflows when their behavior differs. If they share most steps, describe the common prerequisites once and then explain the differences.

## Scientific Simulation Software

Explain the simulated object, model assumptions, configurable parameters, execution process, observables, visualization, data storage, and applicability limits. Give a database or external tool its own section only when the software actually uses it. A general description of a separate tool is not evidence of a product feature.

Do not substitute unsupported scientific conclusions for software documentation. If background literature is required, research and cite it separately; keep the registration manual focused on the software's implementation and operation.

## General Business Software

Organize modules around roles and tasks, such as accounts and permissions, data entry, search and filtering, workflow actions, reporting, import and export, and logging. Each module must have corresponding evidence in source code, routes, menus, or authentic screenshots.

## Figures and Tables

- Use an architecture or module diagram when the structure is difficult to explain in prose.
- Use a flowchart when processing has a meaningful sequence or branch.
- Use a table for comparable environment, parameter, or dataset values.
- Prefer authentic interface screenshots when explaining functions and operations.
- Number figures and tables in order of appearance, and keep body references, captions, and contents consistent.

Each figure should perform one clear explanatory job. Remove unrelated personal information, secrets, internal addresses, and third-party account details from screenshots.
