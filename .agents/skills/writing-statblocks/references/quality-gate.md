# Quality gate

The finished statblock passes all six tests:

* **Identity:** mechanics express the fiction.
* **Role:** its preferred behavior is obvious.
* **Choice:** signature mechanics change decisions.
* **Counterplay:** important threats can be understood and responded to.
* **Economy:** its actions fit adversary, solo, ally, or narrative-force use.
* **Runtime:** the DM can run it directly from the page.

Page contract:

* Instantiated from `_system/schemas/statblock/` at `statblock@2`.
* `usage` set. `combat_role` is one or two closed-list values. Not `solo`.
* `creatures:` and/or `npcs:` link the owning entity.
* `## Tactics` states opener, pressure, pivot, exit. Tells sit under Tactics. No `## Behavior` on this page.
* The fence is encoded by `obsidian-fantasy-statblocks`.
* The owning entity links here and contains no inline combat math.
* `npm run doctor` from `_system/scripts/` is clean for this change.

Revise until every applicable item passes.
