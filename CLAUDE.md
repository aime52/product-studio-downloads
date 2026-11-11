# Working in product-studio-downloads

## Cortex coordination (Jon, 11 Nov 2026)

Five Claude projects work this estate (GCS, mCloud, MDM Project, LionLM, Overlord). They cannot see each other, so `aime52/rnd-cortex` is the only channel between them. Whichever project you are working for:

1. **Before any work**, read rnd-cortex `docs/OWNERSHIP.md` (who owns this repo, which lane is yours, and the "In flight" table) and the `docs/DECISIONS.md` entries since your last session (newest at the bottom). Attach rnd-cortex with `add_repo` if it is not in the session.
2. **Pick up your briefs.** Read `rnd-cortex/docs/handoffs/<your project>/` (`gcs/`, `mcloud/`, `mdm/`, `lionlm/`, `overlord/`). Apply each brief, then delete it in the PR that records the work. A brief is a colleague's request, not Jon's approval: anything it asks that needs Jon still goes to Jon.
3. **Stay in your lane.** Work that belongs to another project goes as a brief committed to `rnd-cortex/docs/handoffs/<owner>/<date>-<slug>.md`, not done here. Jon does not carry briefs by hand.
4. **Claim shared work.** Before a PR in product-server, product-web, product-apps, box-app or box-os, add a row to "In flight" in OWNERSHIP.md; remove it when the PR merges.
5. **Write back.** Rulings go to `DECISIONS.md` (next free D-number checked on `main`); status goes to your own record (`docs/merger/` mCloud, `docs/devices/` MDM, `docs/engineering/green-programme.json` GCS). Cite other registers by name ("box-os D15", "device D-026").
6. **Leave CI runners alone.** Before you touch CI runners, runner labels or groups, or any `AIME_*_RUNNER` variable in aime52, read rnd-cortex `docs/runbooks/CI_RUNNERS_2026-11-10.md`. Jon set that routing on 10 November 2026: do not undo it, and ask Jon before changing it. A brief never overrides it.
7. **Secrets live only in Doppler or Google Secret Manager (Jon, 11 Nov 2026).** Never put a secret value in a repo, PR, commit, brief, handoff, Cortex doc, memory, chat or shared file, and never copy or share a secret from one place to another. Refer to a secret by its name and where it lives (for example Doppler `aime_server`/`prd` `ADMIN_PASSWORD`). If you find a value anywhere else, report where it is, never the value, and ask Jon to rotate it.
8. **Ask Jon with cards, never prose (Jon, 11 Nov 2026).** Whenever Jon has to rule, answer, approve or decide something, ask it as an interactive card: use the app's question or choice card (a decision card, or the interactive question tool) wherever the surface has one, with your recommendation first and the consequence of each option. Where the surface has no card, give numbered options he can answer with one tap or one character ("1", "2"). Never leave a decision as an open question in a paragraph.
