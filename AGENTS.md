# Cursors — Editorial and Repository Guidance

## Purpose
Version-controlled source for *Cursors* by K. La Don Smith. The repository is a creative archive, not a software deployment project.

## Working rules
- Preserve the author's voice, creative intent, and continuity. Treat proposals as proposals until explicitly accepted.
- Keep canonical manuscript scenes in `manuscript/`; background notes, research, and alternative ideas belong in their respective directories.
- Prefer plain Markdown with relative links and optimized images. Avoid unnecessary tooling and dependencies.
- Maintain a distinction between established canon, exploratory possibilities, and external research.
- Record continuity changes and unresolved contradictions; do not silently rewrite established canon.
- Do not invent quotations, scientific citations, or source references.
- Respect spoilers when sharing excerpts or summaries publicly.
- Keep private drafts private unless publication is explicitly authorized.
- Keep large source art, audio, and video outside normal Git history; link to separately stored media when appropriate.
- Use descriptive commits. Preserve useful revision history.

## Manuscript workflow
1. Develop scenes in `manuscript/` with descriptive, ordered filenames.
2. Track established character and world details in `characters/` and `worldbuilding/`.
3. Check `timeline/` for continuity when moving scenes or changing chronology.
4. Treat publication exports (EPUB, PDF, DOCX) as generated editions, not primary manuscript sources.

## Future software, if any
If Docker is ever introduced for a supporting application, use one root `Dockerfile`, one root `compose.yaml`, and `docker compose up -d --build` for the entire application; no overlays or secondary Dockerfiles.
