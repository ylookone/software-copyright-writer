# Source Code and Document Identification Materials

Use this reference when preparing source code, determining document length, or selecting a deposit method. It summarizes baseline rules and a reliable preparation method. Verify the current requirements of the actual filing channel before formal submission.

## Baseline Official Rules

As verified on 2026-09-11, Articles 9 through 11 of the Measures for the Registration of Computer Software Copyright state that a standard application includes the application form, software identification materials, and relevant supporting documents. The identification materials consist of source code and one form of software documentation. The ordinary deposit uses the first and last 30 consecutive pages of each; if the complete program or document has fewer than 60 pages, the complete material is submitted. Except in specified cases, program pages contain at least 50 lines and document pages at least 30 lines. Article 17 specifies A4 paper.

Official sources:

- National Copyright Administration, Measures for the Registration of Computer Software Copyright: https://www.ncac.gov.cn/xxfb/flfg/bmgz/202410/t20241015_869486.html
- National Laws and Regulations Database, Regulations on Computer Software Protection: https://xzfg.moj.gov.cn/front/law/detail?LawID=913

These provisions do not contain every operational requirement of every filing channel. Recheck official sources for online form fields, signatures or seals, file formats, and exceptional deposit methods. Do not use a commercial filing agent as the sole authority.

## Preparing the Source Code

1. Identify the code state that corresponds to the registered version and record its commit, release, or archive source.
2. Build an inventory of application-owned source files. Exclude third-party dependencies, virtual environments, build output, caches, downloaded models, generated files, binaries, and test data.
3. Arrange files in a stable order that exposes the entry point, core business logic, and major output paths. Retain the complete ordering list.
4. Treat the ordered files as one continuous program sequence, then select consecutive beginning and ending pages according to the applicable rule. Do not assemble arbitrary, unrelated fragments.
5. Preserve valid code and comments. Do not duplicate code, pad blank lines, fabricate implementation, or insert unrelated code to reach a page target.
6. Check for keys, tokens, passwords, personal data, internal addresses, and private data paths. Explain the effect before redaction or an exceptional deposit, and follow the official rule that applies.

Use the user's template or the filing channel's instructions for page headers, footers, file paths, page numbers, software name, and version. Do not describe a common formatting convention as a statutory requirement.

## Preparing the Documentation

The design specification or user manual must be authentic documentation for the registered software, and its deposited beginning and ending pages must remain consecutive. When the complete document is shorter than the applicable threshold, preserve the complete document instead of padding it with repeated screenshots, generic background, or oversized text.

Before delivery, confirm that the source code and documentation belong to the same version and that the modules, interfaces, databases, models, and export functions described in the document are traceable to the project.
