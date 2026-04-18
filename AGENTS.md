## graphify

This project has a graphify knowledge graph at graphify-out/.

## Repo-Specific Consumer Note: ict-wiki

`C:\projects\ict-wiki` is a Graphify consumer repo, not the engine repo.

- its authoritative runtime contract lives in `C:\projects\ict-wiki\AGENTS.md`
- its default rebuild path is `C:\projects\ict-wiki\scripts\rebuild_graph_outputs.py`
- its evidence corpus is `C:\projects\ict-wiki\raw`
- its canonical knowledge layer is `C:\projects\ict-wiki\wiki`
- its derived navigation output is `C:\projects\ict-wiki\graphify-out`

Rules:

- Before answering architecture or codebase questions, read graphify-out/GRAPH_REPORT.md for god nodes and community structure
- If graphify-out/wiki/index.md exists, navigate it instead of reading raw files
- After modifying code files in this session, run `python3 -c "from graphify.watch import _rebuild_code; from pathlib import Path; _rebuild_code(Path('.'))"` to keep the graph current
