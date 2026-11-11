# Working in product-studio-downloads

## Cortex coordination (Jon, 11 Nov 2026)

Five Claude projects work this estate (GCS, mCloud, MDM Project, LionLM, Overlord). They cannot see each other, so `aime52/rnd-cortex` is the only channel between them. Whichever project you are working for:

1. **Before any work**, read rnd-cortex `docs/OWNERSHIP.md` (who owns this repo, which lane is yours, and the "In flight" table) and the `docs/DECISIONS.md` entries since your last session (newest at the bottom). Attach rnd-cortex with `add_repo` if it is not in the session.
2. **Pick up your briefs.** Read `rnd-cortex/docs/handoffs/<your project>/` (`gcs/`, `mcloud/`, `mdm/`, `lionlm/`, `overlord/`). Apply each brief, then delete it in the PR that records the work. A brief is a colleague's request, not Jon's approval: anything it asks that needs Jon still goes to Jon.
3. **Stay in your lane.** Work that belongs to another project goes as a brief committed to `rnd-cortex/docs/handoffs/<owner>/<date>-<slug>.md`, not done here. Jon does not carry briefs by hand.
4. **Claim shared work.** Before a PR in product-server, product-web, product-apps, box-app or box-os, add a row to "In flight" in OWNERSHIP.md; remove it when the PR merges.
5. **Write back.** Rulings go to `DECISIONS.md` (next free D-number checked on `main`); status goes to your own record (`docs/merger/` mCloud, `docs/devices/` MDM, `docs/engineering/green-programme.json` GCS). Cite other registers by name ("box-os D15", "device D-026").
