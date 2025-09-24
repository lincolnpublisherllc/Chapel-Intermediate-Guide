README (requested “out here”)
What you’re getting

A folder per chapter: Chapter_01, Chapter_02, …

Inside each folder are the code snippets that appear in that chapter.

Filenames are taken from nearby hints in the text when available (for example, lines like core.chpl — pure domain logic). When no clear name was present, I used sequential names like snippet_01.chpl, snippet_02.c, etc.

Non-Chapel snippets that appear in the book (C headers/sources, shell scripts, Mason.toml, small CSV examples) are included with the correct extensions.

Quick stats (from the manifest)

Total chapter folders: 28

Total extracted files: 406

The JSON manifest lists every file under each chapter folder so you can cross-check easily.

How I mapped things

Chapter detection: Based on headings like “chapter 1”, “chapter 2”, etc.

Filename detection: If the surrounding paragraph referenced a path or file name (e.g., src/logkit.chpl, fnv.c, Mason.toml), I used that. Otherwise I assigned snippet_XX.*.

Language detection:

Chapel: default when code looked like Chapel (module, proc, iter, forall, use, {}, ;).

C / headers: lines with #include, extern, or typical C signatures.

Shell: #!/usr/bin/env bash.

TOML: lines like name = "...", [dependencies].

CSV example rows: dated lines like 2025-09-01,/home,200.

Known limits and notes

Some chapters are conceptual and may have no true “code blocks,” so their folders may be empty.

A few snippets in the book are shown in prose style rather than fenced blocks; I used careful heuristics to capture those. If you see a snippet that should be split into two files or renamed, tell me what to call it and which chapter it belongs to, and I’ll update the ZIP accordingly.

Everything was extracted from your uploaded file “Chapel Intermediate Guide.docx.” 

Chapel Intermediate Guide

Suggested next steps

Open the JSON manifest to spot-check chapter contents quickly.

If you want the filenames to match the book’s internal layout exactly (for example, src/…, test/…, examples/…), I can re-organize the ZIP to that structure.
