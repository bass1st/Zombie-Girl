# game_brief

GitHub-friendly Markdown conversion of the current **Zombie Girl: Morrowsoil** MVP design document.

This file is intended to act as a single-source brief for design, writing, art, UI, engineering, production, and AI coding-agent handoff.


Zombie Girl: Morrowsoil

Ultimate Composite MVP Design Document

Current-state game direction for design, writing, art, UI, engineering, production, and AI coding-agent handoff

| Field | Value |
| --- | --- |
| Project codename | Zombie Girl: Morrowsoil |
| Audience | Development department planning and AI coding-agent understanding |
| Status | Current-state MVP design-definition snapshot |
| Recommended genre label | Story-driven tactical puzzle adventure with light action-RPG and light survival pressure |
| Recommended camera | 2D top-down oblique / three-quarter view / quarter-view |
| Playable lead | Lottie Harrow |
| Current purpose | Give one self-contained Word file that explains the entire current project state so far |

## Contents

## 1. Document purpose and usage

## 2. Simple answer sheet

## 3. Professional recommendation

## 4. Current lock status and readiness

## 5. Game pillars

## 6. MVP scope

## 7. Genre and camera specification

## 8. Core loop

## 9. Core mechanics family

## 10. Combat specification

## 11. Puzzle specification

## 12. Inventory, progression, and survival pressure

## 13. World and lore model

## 14. Factions

## 15. Character bible

## 16. Story structure

## 17. Region structure

## 18. Art direction

## 19. UI and UX direction

## 20. Audio direction

## 21. Technical architecture for AI coding agents

## 22. Vertical slice recommendation

## 23. Risks and anti-patterns

## 24. Open decisions

## 25. Final project summary

## Appendix A. Reference interpretation notes

## Appendix B. Immediate next work items

## 1. Document Purpose and Usage

Purpose: This file is the current single-source design document for Zombie Girl: Morrowsoil. It exists to explain the entire present project state in one place so that a human department lead, producer, or AI coding agent can understand the game without needing additional conversation context.

Interpretation rule: This is not a final production schedule and not a full franchise bible. It is a structured MVP design document. Anything described here should be treated as current direction unless it is explicitly marked as movable, deferred, or open.

Use this file to align design, writing, art, UI, engineering, and production on the same present-state understanding.

Treat percentages in this document as design-definition readiness, not implementation completion.

Treat locked names and concepts as stable unless the document marks them as adjustable.

Assume the game must work as a fully stand-alone product even if its hidden origin can later connect to wider multiversal lore.

Assume the target is a highly memorable indie-scale game with a small protagonist, iconic mechanics, and a very clear authored identity.

## 2. Simple Answer Sheet

| Question | Current answer |
| --- | --- |
| Genre | Story-driven tactical puzzle adventure. This is the main label. It can also be described as a puzzle-adventure game with light tactical combat, light RPG progression, and light survival pressure. |
| What it is not | Not a stat-heavy action RPG. Not a harsh survival simulator. Not a large party tactics game. Not a pure side-scrolling action game. |
| Core play loop | Explore -> observe anomaly -> solve traversal or puzzle problem -> enter a small tactical encounter or escape sequence -> collect salvage or clue -> return to safe route -> unlock the next story gate. |
| Main character | Lottie Harrow, a zombie-born small girl. Quiet, cheerful in a private way, behaviorally unserious, but actually highly observant. |
| Primary goal | Investigate wrong-death anomalies, uncover the human underground restoration plan called Redemption, and stop the Dawn Bell before it erases surface zombie civilization. |
| Recommended camera | 2D top-down oblique / three-quarter view / quarter-view. This is the closest technical name for the camera angle the user has been describing. |
| Overall feel | Cartoonish, eerie, dusty, warm, lonely, and mechanically readable. |

Professional recommendation: The project should be pitched internally as a tactical puzzle adventure first. That phrasing protects the game from genre confusion and keeps the team from accidentally building three incompatible games at once.

## 3. Professional Recommendation

### 3.1 Camera recommendation

The reference cluster points more strongly toward a 2D oblique three-quarter camera than toward a pure side view. This view is sometimes casually called quarter view. It is not strict isometric. It is closer to top-down oblique, three-quarter RPG view, or isometric-adjacent 2D adventure framing.

Use the three-quarter view for exploration, puzzle spaces, and tactical encounter rooms so the world stays visually coherent.

Reject pure side view as the main MVP format because it weakens environmental legibility, settlement density, and tactical readability.

Side-view sequences are acceptable only as dream scenes, flashbacks, or highly controlled sub-modes.

### 3.2 Genre blend recommendation

The best professional modification of the user preference is not to force the game into a conventional “action RPG” or “survival game” bucket. The cleaner answer is a story-first puzzle adventure with tactical combat encounters. This is more achievable for an indie pipeline and more faithful to the two identity pillars: zombie protagonist and small girl protagonist.

Story layer: authored narrative, chapter progression, emotional scenes, and dream sequences.

Puzzle layer: the same core mechanics used in battle also solve traversal, infiltration, and environmental logic problems.

Tactical combat layer: small encounter boards inspired by the “combat as puzzle” feel of Mario + Rabbids rather than large-scale party warfare.

Light RPG layer: a few upgrades, encounter tools, and story-gated expansions. No heavy stat spreadsheet.

Light survival layer: resource pressure exists, but there is no hunger-thirst micromanagement.

### 3.3 Reference synthesis

From Mario + Rabbids, borrow battle-as-puzzle clarity. From Wizard with a Gun and similar top-down oblique references, borrow exploration readability and stylized UI confidence. From Backbone, SANABI, Katana Zero, and The Coffin of Andy and Leyley, borrow mood discipline and strong framing. From Breath of Fire IV, borrow authored encounter logic and readable tactical staging. Do not copy any one title directly.

## 4. Current Lock Status and Readiness

| Category | Current state |
| --- | --- |
| Locked | Lottie Harrow, Nib, Kindly, Jonah Harrow, Mara Harrow, Ivo Quill, Morrowsoil as world identity, the Pale Quarter as the human underground, Redemption as the restoration program, Dawn Bell as the machine-scale threat, Bone Orchard Mother as the in-game title for the death presence. |
| Strong but movable | Main human antagonist exact name, wandering trader exact name, local elder exact name, recurring hunter exact name, archivist exact name, region names beyond Haywake and Pale Quarter if desired. |
| Open / deferred | Final shell upgrade names, exact enemy roster size, exact number of boss-grade encounters, final art pipeline, final engine if the studio already has a house standard. |

Readiness meaning: The following percentages estimate how defined each domain is on paper right now. They are not development completion percentages.

| Design domain | Readiness | Meaning |
| --- | --- | --- |
| World premise and core lore | 80% | Setting identity, species logic, and hidden-origin model are substantially defined. |
| Narrative spine / main story | 70% | Beginning, reveals, final conflict, and central theme are defined enough for chapter planning. |
| Lead character identity | 85% | Lottie is already clear in concept, tone, and story function. |
| Major supporting cast concepts | 45% | Functions are defined; naming and detailed arcs remain partially open. |
| Camera / genre / macro direction | 75% | The recommended view and genre stack are clear. |
| Core mechanical identity | 60% | The iconic mechanic family is defined in principle but still needs tuning and prototype proof. |
| Combat implementation detail | 40% | Turn flow and room logic are sketched, not production-final. |
| Puzzle implementation detail | 45% | Puzzle verbs and quality rules are clear, but content patterns are not fully expanded. |
| Progression / economy | 35% | Enough exists for MVP definition, not enough for balancing. |
| UI / HUD direction | 35% | Visual goals are visible from references, but concrete wireframes remain early. |
| Art pipeline definition | 30% | Style direction is strong; pipeline and staffing rules are not final. |
| Technical architecture | 30% | Enough exists for AI-agent scaffolding, not enough for final engineering lock. |
| Production planning | 20% | Useful for sequencing discussion, not yet a full schedule. |

## 5. Game Pillars

Pillar A: small girl, oversized consequence. The player is a small girl, and that must be mechanically meaningful. Size affects movement, recoil, hiding, vulnerability, and the emotional shape of every encounter.

Pillar B: zombie-born perspective, not human guilt cosplay. The game is not about a monster proving she is basically human. It is about a child of the successor world who does not need old humanity’s permission to exist.

Pillar C: one mechanic family used everywhere. Traversal, puzzles, infiltration, and combat must all use the same small family of iconic mechanics. This is essential for MVP clarity and memorability.

Pillar D: eerie but warm. The mood is not grimdark nihilism. The world is dead-adapted, but it is also inhabited, domestic, and unexpectedly tender.

Pillar E: stand-alone surface, hidden deep link. The game must be fully understandable with zero Zaruverse knowledge. Any deeper cosmological connection stays optional.

## 6. MVP Scope

Target campaign length: approximately 5 to 7 hours on a first clear.

Chapter count: prologue plus 5 main travel chapters plus 1 final chapter.

Playable lead count: 1. Lottie only.

Persistent support companion: Nib.

Human ally with recurring dialogue and scene support: Ivo Quill.

Core regions for MVP: Haywake, one rail or trade region, one drowned or marsh region, one archive or observatory region, the Pale Quarter, and the Dawn Bell finale zone.

Mechanical pillars for MVP: three-quarter exploration, tactical encounter rooms, Nib scouting, Stillness, Scent, Kindly/Recoil, clue collection, authored dialogue, one ending.

Scope rule: The correct MVP is compact, authored, and mechanically memorable. Every proposed feature should be checked against the pillars before it is accepted.

Out of scope: Explicitly out of scope for MVP: open world design, multiplayer, base building, giant crafting trees, party tactics with several playable units, branching faction campaigns, procedural roguelike campaign structure, and stat-heavy rarity systems.

## 7. Genre and Camera Specification

Final genre phrase: story-driven tactical puzzle adventure with light action-RPG and light survival pressure.

Camera definition: 2D top-down oblique / three-quarter view. The environment reads like a slightly angled RPG map, not a strict side view and not true isometric. The camera must favor readability of terrain edges, low obstacles, cover points, small gaps, and pathing lanes.

Use stylized 2D illustration with high silhouette clarity and expressive character animation.

Avoid hyper-real texture noise. The world should stay readable at indie production scale.

Do not commit to pure retro pixel art if the project wants expressive cartoon acting. A hand-drawn or painted 2D pipeline will support Lottie better.

If pixel influence remains desirable, keep it in UI accents, portraits, or special dream scenes rather than as the project-wide limitation.

## 8. Core Loop

Enter a region or story chapter.

Observe environmental wrongness: preserved corpses, white growths, hidden broadcasts, route anomalies, or human-clean machinery.

Use movement, Stillness, Scent, Nib, and Kindly to navigate hazards and gather information.

Resolve tactical encounter rooms or stealth escapes.

Collect salvage, clues, or upgrades.

Return to a safe space, story gate, or key NPC conversation.

Unlock the next region or truth layer.

Minute to minute, the player should move, observe, test, manipulate, and decide whether to engage or bypass. The reward for success is not only loot; it is also space, story progress, and understanding.

## 9. Core Mechanics Family

### 9.1 Stillness

Stillness is Lottie’s ability to drop into an inert corpse-like state. Because she is zombie-born, this is not a disguise skill. It is a native body state. In gameplay, Stillness is used for stealth, enemy manipulation, pressure reset, sensor bypass, and specific puzzle interactions.

Ferals deprioritize or ignore Lottie in Stillness unless directly touched or unless the state is broken by obvious stimulus.

Some human detectors look for warmth, pulse, or living motion and can be bypassed by Stillness.

Certain conveyors, carts, rafts, or machine channels can move Lottie when she is Still because she reads as cargo or corpse matter.

In tactical rooms, entering Stillness can break target locks, alter aggro, or bait enemy movement.

### 9.2 Scent

Scent is the environmental manipulation system tied to Lottie’s undead nature. She can interpret rot trails, carry simple lure compounds, and use odor logic to redirect or reveal things.

Scent can lure ferals away from a route or toward a trap.

Scent can activate rot-grown mechanisms or reveal fungal paths invisible to ordinary sight.

Scent can contaminate cover or terrain, changing enemy behavior during tactical encounters.

Human-clean spaces react negatively to Scent, making it a risk inside the Pale Quarter.

### 9.3 Kindly / Recoil

Kindly is the oversized shotgun. The gun is not just damage output. Its recoil is one of the game’s central verbs. Because Lottie is small, every shot is also movement, force, and puzzle logic.

Firing Kindly pushes Lottie opposite the shot direction unless she braces against a wall, anchor point, or heavy object.

Recoil can cross short gaps, slam Lottie into platforms, or snap her behind cover.

Shots push enemies, break fragile matter, trigger switches, or open soft barricades.

Puzzle spaces and combat arenas should be designed around this same force logic.

### 9.4 Nib

Nib is both companion and mechanics amplifier. In systems terms, he provides scouting, remote peck interactions, clue highlighting, omen behavior, and occasional route suggestions.

Nib can scout a short distance into vents, rafters, holes, or bushes to mark interactables.

Nib can peck exposed switches, pull tiny items, or harass fragile targets.

Nib’s behavior also foreshadows hidden danger, threshold scenes, and the Bone Orchard Mother presence.

Mechanic-family rule: Every mandatory puzzle and every tactical room should use at least two of the following: movement, Stillness, Scent, Nib, Kindly/Recoil. If a room only uses generic key-door logic, it is too weak for this project.

## 10. Combat Specification

Combat should feel like a small tactical encounter puzzle, not a conventional action combo game. The player is rewarded for positioning, force manipulation, baiting, and route control.

Exploration is real-time.

When Lottie enters a battle trigger or is discovered in a hostile zone, the current room shifts into tactical turn mode.

The battlefield remains the same map space; there is no separate JRPG battle screen.

Each encounter room should be small enough to read instantly and rich enough to solve in more than one way.

| Variable | Recommended MVP rule |
| --- | --- |
| Move phase | Lottie gets one move phase per turn within a visible movement radius. |
| Action points | Lottie gets 2 AP per turn. |
| Typical AP costs | Shoot 1 AP; item 1 AP; interact 1 AP; enter Stillness 1 AP; Nib command usually free or once-per-turn. |
| Cover | Low cover, full cover, no cover. Lottie’s small body makes low cover especially valuable. |
| Enemy turns | Enemies act in simple readable sequences. Ferals prefer smell and motion. Human units prefer line-of-fire and suppression. |
| Victory states | Defeat hostile units, escape to exit node, survive a fixed turn count, or complete the room objective. |

Combat mechanics must express the concept. Small body means low objects matter as cover. Zombie body means Stillness and special environmental tolerance matter. Oversized shotgun means space changes when the player attacks.

Readability rule: Enemy counts must stay low in MVP. Quality of puzzle pressure is more important than quantity of units.

| Enemy archetype | Function |
| --- | --- |
| Feral shambler | Simple smell-and-motion pursuer; teaches Scent and Stillness. |
| Pouncer / leaper | Punishes exposed routes and forces cover planning. |
| Bell drone / detector | Human surveillance device that punishes noise or pulse and encourages Stillness. |
| Quarter rifle unit | Human clean-shot soldier who values line-of-fire and cover discipline. |
| Quarter purifier | Uses white-agent clouds or sterilizing tools that reshape the room. |
| Heavy / sentry | Static threat that creates forced movement puzzles rather than merely dealing damage. |

## 11. Puzzle Specification

Puzzles must feel like the world was built for this exact protagonist. They should not feel like generic imported mechanics. A strong puzzle always asks what a small undead girl with a bird and a shotgun can do here that another hero could not.

Route puzzles: pathfinding through small gaps, conveyors, low-cover lanes, and corpse-cargo channels.

Force puzzles: using Kindly’s recoil or enemy push to move self, objects, or hazards.

Attention puzzles: manipulating feral or human behavior with Stillness, Scent, light, or noise.

Threshold puzzles: crossing zones that read differently for living and undead bodies.

Dream or omen puzzles: short surreal spaces that communicate Bone Orchard Mother presence or death-law contradictions.

Quality rule: A good puzzle teaches through consequence, not lecture. If a room can be solved by only shooting everything, it is not a good representation of the game’s identity.

## 12. Inventory, Progression, and Survival Pressure

This game should not become a hard survival-management simulator. The correct design is light survival pressure: enough scarcity to make field decisions meaningful, not enough bookkeeping to bury the story.

Keep inventory small and readable.

Use only a few item classes: shells, lure compounds, patch kits, keys, salvage, and story items.

Inventory pressure should reinforce “small girl protagonist” without becoming annoying.

Use a compact health model such as segmented hearts or a short durability bar rather than RPG hit point sprawl.

Failure should reset to recent checkpoints with fast reload. Long corpse-runs are not appropriate.

| Progression lane | MVP recommendation |
| --- | --- |
| Kindly upgrades | A few story-gated upgrades such as brace shot, slug shot, or utility shell types. |
| Nib upgrades | Longer scout range, remote switch peck, clue pulse. |
| Lottie traits | Improved Stillness duration, stronger scent interpretation, or specific environmental tolerance. |
| Narrative progression | Dialogue flags and region unlocks matter as much as pure mechanics. |

## 13. World and Lore Model

Morrowsoil is a dead-adapted Earth-analog where humans collapsed, zombies inherited the surface, and civilization slowly reformed under the wrong species label. The player does not need any outside franchise knowledge to understand this.

Hidden-origin rule: The hidden-origin explanation is that a black foreign object fell to Earth in the old age. Human institutions recovered it, studied it, and exposed the planet to an impossible material called Morrow Seed. For stand-alone players, this is just the thing from the sky. For deeper franchise use, it can later be interpreted as a foreign reliquary or cross-reality object. That deeper layer must remain optional.

This is not a standard virus story. Morrow Seed rewrote the boundary between death, memory, decay, and adaptation. The first generations were catastrophic. Over time, the dead stabilized. The world is therefore in a successor-species phase, not merely an outbreak phase.

Warm Age: ordinary human civilization.

Black Cradle Fall: the foreign object is recovered in secret.

Break Years: containment failure and misuse spread the death-adaptation event.

Famine Wars: human collapse accelerates through panic, war, and scorched-earth responses.

Quiet Rot: zombie populations slowly stabilize.

Hearth Age: settlements emerge, trade returns, and local memory cultures form.

Firstborn Year: Lottie is born from two zombie parents, proving successor continuity.

Zombies are not one thing. There are feral, settled, and born-dead states.

Older zombies often suffer memory damage and identity drift. Lottie does not, because she was never interrupted by prior human death.

Settled zombies are not defined only by flesh-eating. Their societies use agriculture, fungi, rendered oils, scavenged food chains, and maintenance rituals.

New zombification is no longer the daily global threat. The story happens after civilization has partially re-formed.

Humans underground are restorationists, not just survivors.

## 14. Factions

Surface settlements are not evil inversions of human towns. They are fragile, practical, rural, and often emotionally subdued because of memory damage and survival logic. They must feel worth saving.

The Pale Quarter is the human underground restoration state. It is clean, doctrinal, technologically advanced, and politically theological. Its people believe the world is fallen because death was allowed to continue incorrectly.

Core belief: Redemption means correcting unfinished death.

Practical expression: build and fire the Dawn Bell, sterilize adapted undead life, reclaim the surface.

Moral function: the humans are not cartoon monsters. They are possessive custodians.

The Bone Orchard Mother should not behave like a faction leader. She is an observing law. In deep canon this can map to Kythene, but in the game itself she should stay eerie, brief, and optional in explanation.

## 15. Character Bible

Lottie Harrow: lead protagonist. Around 12 to 14 in readable age. Small, hat-brim silhouette, patched farm-western clothing, oversized shotgun, quiet-bright behavior, sharp pattern recognition.

Behavioral summary: cheerful yet quiet, does what she wants, cares intensely about specific people, does not perform intelligence, is actually highly observant.

Narrative function: proof that zombie civilization is no longer only a remnant; it is becoming a people.

Mechanical function: the body through which Stillness, Scent, and Kindly/Recoil become coherent.

Nib: companion crow with a suspicious skull-cap mask. Cute, useful, and quietly uncanny. Surface read: mascot-companion, scout, mood-setter, route helper. Deeper read: grave-familiar carrying death’s tracking logic, possibly connected to the Bone Orchard Mother.

Kindly: Lottie’s oversized shotgun. Not just a weapon, but a force-logic device. The name should stay. It is one of the project’s strongest tonal details.

Jonah Harrow: Lottie’s father. Repairman, fence-builder, quiet protector, one of the earliest settled zombies in the home region. Represents practical survival without speeches.

Mara Harrow: Lottie’s mother. Schoolkeeper, record-keeper, song-carrier, and soft curator of local truth. Represents love through careful concealment.

Ivo Quill: human youth from the Pale Quarter. Educated, brittle, precise, awkward aboveground, and initially loyal to the restoration narrative. His arc is discovering that the underground preserved ownership, not moral superiority.

Main human antagonist: exact final name is still movable, but the concept is stable. Calm, refined, almost maternal, and absolutely committed to Redemption. She must sound merciful while planning species erasure. She does not hate Lottie; she pities her.

Wandering trader: exact final name is movable. Concept is stable: dusty road veteran, mobile world-linker, practical storyteller, and route stabilizer. Makes the world feel connected through trade and rumor.

Recurring hunter from the Pale Quarter: exact final name is movable. Concept is stable: precise operational hand of the doctrine, clean field agent, and recurring pressure body. Polite and frightening rather than loud.

Archivist / truth-keeper: exact final name is movable. Concept is stable: half-broken witness living near the old research scar, carrying damaged memory of the origin and recognizing Lottie as a new condition rather than a symptom.

Bone Orchard Mother: brief recurring presence. Ancient, calm, rural-death-coded, and never overexplained. Appears in dreams, threshold moments, and nearly impossible survivals. In deep canon this can map to Kythene, but in play it remains image and omen first.

## 16. Story Structure

Story statement: a zombie-born farm girl travels across the inherited dead world after noticing death behaving incorrectly, discovers that the last human underground civilization is preparing a purification event called Redemption, and fights to stop a restoration machine that would erase her people from history.

| Chapter | Purpose | Main reveal or function |
| --- | --- | --- |
| Prologue: Haywake Morning | Establish home, warmth, and basic mechanics | Lottie is ordinary inside an extraordinary species-history. |
| Chapter 1: The Wrong Deer | Introduce preserved-death anomaly | Something is reversing decay incorrectly. |
| Chapter 2: The Rattleline Road | Teach travel and tactical encounters | Other settlements report related disturbances. |
| Chapter 3: Drowned / Marsh Region | Expand world and human trace evidence | The underground still reaches upward. |
| Chapter 4: Archive Scar | Origin truth layer | Humans studied the sky-object first; the world fell through ownership. |
| Chapter 5: Pale Quarter Infiltration | Reveal the doctrine and the plan | Redemption and the Dawn Bell are real and imminent. |
| Chapter 6: Return and Warning | Social conflict and coalition building | Not all surface people respond well; fear divides survival societies. |
| Final Chapter: The Dawn Bell | Climax and philosophical confrontation | Lottie rejects the idea that her existence needs human permission. |

Theme guardrail: the emotional center of the game is not “a monster proving she is human.” The emotional center is “a new child insisting that being new does not make her invalid.”

Recommended ending: Lottie disrupts the Dawn Bell using the contradictory resonance of her own born-dead state, creating a broken signal event that prevents immediate extinction, exposes the hidden infrastructure, and forces the world into a new era of open conflict and negotiation. The ending should not fully solve species politics. It should stop erasure and begin history.

## 17. Region Structure

| Region | Role in campaign | Mechanical emphasis |
| --- | --- | --- |
| Haywake | Home region and emotional baseline | Basic movement, Nib, first use of Kindly, first anomaly. |
| Rail / trade region | World connectivity and travel pressure | Cover, recoil movement, first tactical skirmishes, trader contact. |
| Drowned or marsh region | Atmosphere escalation and hidden infrastructure | Stillness routes, scent puzzles, surveillance hints. |
| Archive scar / observatory region | Origin truth and history excavation | Environmental storytelling, archive puzzle logic, archivist scenes. |
| Pale Quarter | Human doctrine reveal and infiltration | Detector systems, sterile hazards, tight tactical rooms. |
| Dawn Bell finale zone | Climax and machine-scale confrontation | Everything combined: recoil, stillness, scent, Nib, timed objectives. |

The MVP does not need many biomes. It needs a small number of strongly contrasted spaces with memorable rules and visual identity.

## 18. Art Direction

Visual north star: cartoonish but not unserious. Dusty, readable, slightly storybook, and capable of quiet dread.

Lottie must have a silhouette readable at tiny scale: strawhat, small body, oversized shotgun.

Nib must be visually cute at first glance and wrong on second glance.

Human-clean antagonists should contrast sharply with the organic clutter and patched domesticity of the surface.

Invest in expressive cut animation: hat bounce, reload posture, cautious step, limp Stillness drop, small recoils, and Nib reactions.

Use animation to sell intelligence without over-dialoguing it. Lottie should often think through posture and pause.

Bone Orchard Mother scenes should feel like visibility errors, not boss cinematics.

Surface zones should feel lived in by the dead: farms, patchwork structures, fungi, rails, marsh lanterns, reused machinery.

Pale Quarter spaces should feel clinically filtered, white, vertical, and doctrinal.

## 19. UI and UX Direction

Readable at small scale.

Stylized enough to feel authored, never so decorative that tactical information becomes unclear.

Warm surface UI and clean Pale Quarter UI can differ slightly to reinforce the world contrast.

| Required HUD element | Need |
| --- | --- |
| Health / durability | Minimal and immediately legible. |
| Shell count | Always visible during tactical play. |
| AP and move phase | Clear when combat mode starts. |
| Nib prompt | Simple icon or hotkey cue. |
| Objective text | Short and non-intrusive. |
| Interact prompts | Consistent and compact. |

UX recommendation: Borrow the confidence of stylized indie UI, but avoid overcomplicated fantasy widgets. For MVP, clarity wins.

## 20. Audio Direction

Music should be sparse, melodic, and region-specific rather than constantly bombastic.

Surface settlements should feel warm, wooden, airy, and imperfect.

Pale Quarter spaces should feel air-filtered, hollow, and almost prayer-like.

Kindly should sound heavy and meaningful, with recoil emphasized more than raw firearm spectacle.

Nib audio should be tiny but memorable: soft clicks, hops, and rare wrong-sounding calls in omen scenes.

## 21. Technical Architecture for AI Coding Agents

Recommended engine: If the team does not already require another engine, the recommended MVP engine is Godot 4.x. The reasons are strong 2D support, good scene organization, low overhead for tactical room logic, data-driven interactions, and good compatibility with AI coding-agent workflows.

| Scene or module | Purpose |
| --- | --- |
| Boot / Main Menu | Startup, options, save slots, credits. |
| Global managers | Save system, audio manager, dialogue manager, quest manager, input manager. |
| World scene | Exploration maps, NPC placement, interactables, region loading. |
| Encounter controller | Converts a live room into tactical turn mode and resolves combat rules. |
| Dialogue layer | Cutscenes, portraits, branching dialogue flags, chapter gates. |
| Dream / omen layer | Special visual sequences for Bone Orchard Mother and threshold scenes. |
| UI layer | HUD, inventory, AP display, objective panels, prompt system. |

PlayerState: position, health, shells, AP state, upgrades, inventory, quest flags, current chapter.

EncounterDefinition: room bounds, objective type, enemy roster, turn order rules, environment objects, win condition, fail condition.

EnemyDefinition: archetype, movement rule, target preference, status immunities, readable telegraph logic.

InteractableDefinition: type, state machine, required mechanic, output event.

RegionDefinition: chapter gate, map list, NPC presence, ambient set, dialogue nodes.

DialogueState: node ID, conditions, results, portrait set, quest results.

| System | Responsibility |
| --- | --- |
| MovementSystem | Exploration movement, collision, small-step traversal, entering Stillness. |
| NibSystem | Scout targets, peck interactions, omen cues, helper markers. |
| KindlySystem | Aiming, firing, recoil resolution, shell types, breakables. |
| ScentSystem | Lure placement, detection radii, odor-triggered interactions, environmental responses. |
| TurnSystem | Combat state machine, move phase, AP use, enemy turns, win/loss checks. |
| CoverSystem | Low cover, full cover, line-of-fire preview. |
| PuzzleSystem | Room-state evaluation, condition tracking, gate unlocks, reset rules. |
| QuestSystem | Story progression, evidence collection, chapter transition. |
| SaveSystem | Checkpoint and full-save serialization. |

Exploration state: free movement, ambient dialogue, inspection, Nib scouting, object interaction.

Alert state: room notices danger, UI signals transition, entities lock into tactical mode.

Player tactical turn: one move phase plus AP spending.

Enemy tactical turn: enemy sequence resolves one archetype at a time.

Resolution state: win objective met, failure state met, or return to exploration.

Build one vertical slice room that supports exploration -> tactical transition -> win condition -> dialogue return.

Implement Stillness, Recoil, and one Nib interaction before adding many enemy types.

Use data-driven encounter definitions so content designers can add rooms without changing core code.

Keep AP, cover, and move ranges visually explicit. Do not hide tactical math.

Prototype with placeholder art early because readability is a core requirement, not a late polish item.

## 22. Vertical Slice Recommendation

The first playable vertical slice should not try to prove the entire game. It should prove the identity loop.

One Haywake-adjacent route.

One wrong-death anomaly.

One puzzle that uses Stillness and Recoil.

One tactical encounter room with 2 to 4 enemies.

One short Nib scout interaction.

One dialogue scene with Jonah or Mara.

One dream or omen flash using the Bone Orchard Mother silhouette.

## 23. Risks and Anti-Patterns

Risk: the team accidentally builds a generic zombie survival game. Counter: keep the successor-species perspective explicit.

Risk: the team accidentally builds a heavy tactics game that loses the intimate story tone. Counter: keep enemy counts low and encounters authored.

Risk: the team overexplains Kythene / Bone Orchard Mother and collapses the game into franchise appendix material. Counter: keep her brief, visual, and optional in explanation.

Risk: the team adds too many weapons or progression systems. Counter: keep Kindly central and upgrades sparse.

Risk: the team treats Nib as only a mascot. Counter: preserve his mechanical utility and suspicious myth role.

Risk: Lottie becomes overly chatty or “TV genius.” Counter: let intelligence live in observation and action, not essay dialogue.

## 24. Open Decisions

Final exact name of the main human antagonist.

Final exact name of the trader, local elder, recurring hunter, and archivist.

Exact shell upgrade list for Kindly.

Exact number of boss-grade encounters for MVP.

Final visual pipeline: hand-drawn sprites, skeletal 2D, or hybrid painted character sheets.

Whether the game includes any optional side stories beyond the main route in MVP.

## 25. Final Project Summary

Zombie Girl: Morrowsoil is a stand-alone story-driven tactical puzzle adventure set in a dead-adapted world where the zombies did not simply ruin civilization; they inherited it. The player controls Lottie Harrow, a quiet, cheerful, zombie-born small girl with an oversized shotgun named Kindly and a suspicious crow companion named Nib. The game is built around three linked mechanics — Stillness, Scent, and Kindly/Recoil — that drive exploration, puzzles, stealth, and tactical encounter rooms. The central story follows Lottie as she notices wrong-death anomalies, uncovers the human underground restoration state called the Pale Quarter, and fights to stop Redemption and the Dawn Bell from erasing the surface people from history. The recommended MVP uses a 2D top-down oblique three-quarter view, compact authored chapters, expressive cartoon animation, low enemy counts, high tactical readability, and a hidden but optional deeper cosmological link that never becomes required knowledge.

## Appendix A. Reference Interpretation Notes

The visual references collectively support a three-quarter exploration camera, stylized HUD, readable tactical overlays, and strong silhouette work.

Mario + Rabbids is the most useful combat-shape reference because it treats encounters as spatial logic problems.

Wizard with a Gun and similar top-down adventure references are useful for readability, atmosphere, and stylized UI confidence.

Backbone, SANABI, Katana Zero, and The Coffin of Andy and Leyley are more useful as tone and framing references than as direct camera or combat templates.

Breath of Fire IV is useful as a reminder that authored, readable, hand-built fantasy logic ages better than overcomplicated system sprawl.

## Appendix B. Immediate Next Work Items

Lock the final core cast names beyond the currently fixed names.

Prototype one exploration room, one tactical room, and one puzzle room using the same mechanic family.

Sketch the exact HUD layout for exploration and tactical mode.

Draft one vertical-slice chapter script from Haywake to the first anomaly scene.

Choose the engine and art pipeline before production staffing expands.
