# Adding more research installments

Perplexity/other agents may produce continuation PDFs, Markdown, code snippets, repositories or new atlases. Preserve all source files with provenance and versioning rather than silently blending them together.

## Intake checklist
1. Assign the next sequential ID: `R04`, `R05`, etc.
2. Record exact original filename, page count/length, SHA-256, source/provider if known, date received and research cutoff if present.
3. Copy the original PDF/attachment under `research/pdfs/` if binary upload is supported. **Do not substitute a reconstructed PDF for the original without labeling it.**
4. Store full searchable plain text in `research/raw-text/Rxx-description.txt`. Note extraction limitations or truncation.
5. Add a row in `docs/RESEARCH-INDEX.md` and update `research/manifest.json`.
6. Extract useful proposed experiments into `docs/EXPERIMENTS.md` with source IDs and evidence levels.
7. Flag disagreements under `docs/OPEN-QUESTIONS.md` rather than overwriting competing claims.
8. Mark whether an invention is duplicate, variant, new, or already built.
9. Never infer missing text after a cutoff; await an actual continuation and link it as a distinct source.

## Required claim prefixes for notes
`[SOURCE-REPORTED]` author/source assertion; `[D]` documented specific result; `[F]` engineering feasible; `[R]` research frontier; `[S]` speculative; `[X]` would require substantial additional machinery; `[VERIFIED]` personally checked against primary source / code / reproducible experiment (include what was checked).

## Source hierarchy
Prefer primary papers, releases, docs, code and repeatable experiments to curated roundups or social-media claims when validating factual assertions. But preserve the wording of user-submitted reports in the raw archive.
