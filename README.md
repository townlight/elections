<a id="civicelections"></a>

# Townlight Elections

Townlight Elections v0.1.1 ships election administration support foundations: cited voter guidance, candidate filing checklists, optional database-backed candidate/canvass workpapers, worker training Q&A, ballot-summary drafts, campaign-finance summaries, canvass checklists, accessibility review, FastAPI runtime, docs, tests, browser QA, and release gates.

It is not a voter registration system, ballot marking device, tabulator, election conduct automation system, campaign finance system of record, official certification workflow, live LLM runtime, or election-system connector.

Install:

```bash
python -m pip install -e ".[dev]"
python -m uvicorn civicelections.main:app --host 127.0.0.1 --port 8141
```

Townlight Elections v0.1.1 is pinned to `civiccore==0.3.0`.

Set `CIVICELECTIONS_WORKPAPER_DB_URL` to persist candidate filing and canvass checklist workpapers. Without it, Townlight Elections remains deterministic and stateless.

## License

Code: AGPL-3.0-only, with the TownLight Public Institution Exception for qualifying deployments. See [LICENSE](LICENSE) and [LICENSE-EXCEPTION.md](LICENSE-EXCEPTION.md).
Documentation: CC BY 4.0 ([LICENSE-DOCS](LICENSE-DOCS)).
