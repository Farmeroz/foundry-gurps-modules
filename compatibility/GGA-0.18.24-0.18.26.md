# GGA 0.18.24–0.18.26 compatibility review

Reviewed 31 October 2026 for the stable GURPS 4e module catalogue.

## Released correction

**Casting Assistant 0.7.1** fixes two integration gaps:

- GGA 0.18.24 supports PDF page labels and custom codes. The assistant previously rejected or split references such as `DFC:A-10` and `DFRPG Spells:20`. Links now preserve those references, registered codes, and embedded colons; numeric ranges still open at the first page.
- GGA 0.18.25 appends GCS usage notes to **melee** attack modes. Saved legacy melee links can recover when exactly one matching annotated mode exists. Exact matches retain priority. Multiple possible matches require the user to choose **Linked attack** and save the profile; the old list position is never used to guess between newly distinguished modes.

The version bump, source changes, tests, README, and user guide are in [Casting Assistant PR #6](https://github.com/Farmeroz/gga-casting-assistant/pull/6).

## Scope of the other-module review

This was a targeted source/dependency review against the stable release changes. It does not certify every Foundry interaction. No additional runtime patch was identified for the changes below.

| Module | Relevant integration reviewed | Result |
| --- | --- | --- |
| GM Control Sheet | Native roll entry point, target range/size modifier helpers, tagged-modifier access | Imported helpers remain available; no patch identified. |
| Ammunition & Resource Assistant | Saved attack references and ranged import modes | The 0.18.25 usage-note change is melee-specific; no ranged-reference migration needed. |
| Casting Assistant | PDF handling, saved melee links, native rolls and modifiers | Two fixes in 0.7.1; modifier entry points remain available. |
| Manual Damage | Native damage roll and Apply Damage Dialog imports | No removed integration entry point identified. |
| Layered Armour | Apply Damage Dialog integration | No removed integration entry point identified. |
| Vitality Reserve | Damage effects and ADD content selection | No patch identified; removing GGA's forced black text merits a theme check. |
| Expanded Criticals | Roll integration | No relevant removed entry point identified. |
| Roll Clarity | Chat/roll integration | No relevant interface change identified. |
| Cone Regions | Region and Manual Damage handoff | No dependency on the changed GGA PDF/combat settings identified. |
| Action Chases | On-the-fly parsing integration | No removed parser entry point identified. |
| Simple Pings | System-independent Foundry integration | No GGA-specific change required. |

GGA 0.18.24 reorganises combat settings and internal combat files. That merits targeted regression checks, rather than automatically changing every module. Its damage-chat change guards item drops without an actor and changes the drop-handler return value; it does not remove the damage rolling entry point used by Manual Damage.

GGA 0.18.25 also fixes self-control-note display and dark-mode text. GGA 0.18.26 updates cover artwork.

## Validation and follow-up

Casting Assistant: formatting, syntax, all **95 automated tests** (including seven new compatibility tests), and ZIP content/integrity checks passed locally and in GitHub's PR workflow. Automated tests use mocks at Foundry integration boundaries.

Focused live checks:

1. Open `B248`, `DFC:A-10`, and a mapped `DFRPG Spells:20` from casting and Grimoire views.
2. Reimport a GCS actor with a unique annotated melee mode. Confirm the profile reconnects. Repeat with multiple possible modes and confirm explicit selection is required, then save and reopen the chosen profile.
3. Compare Casting Assistant and GM Control Sheet targeted rolls against native sheet rolls, including range and size modifiers. Toggle combat options and compare actors inside and outside the encounter.
4. Check ADD, Vitality Reserve, and module windows in light and dark themes, and confirm imported traits retain self-control notes.

Existing Foundry/GGA verified-version metadata is preserved; this source review does not replace live verification. No GGA 1.0 migration is included. Continue tracking that development line separately.

## Upstream references

- [GGA 0.18.24 release](https://github.com/crnormand/gurps/releases/tag/v0.18.24)
- [0.18.23 to 0.18.24 source comparison](https://github.com/crnormand/gurps/compare/v0.18.23...v0.18.24)
- [GGA 0.18.25 release](https://github.com/crnormand/gurps/releases/tag/v0.18.25)
- [GCS melee import change](https://github.com/crnormand/gurps/pull/2994)
- [GGA 0.18.26 release](https://github.com/crnormand/gurps/releases/tag/v0.18.26)
