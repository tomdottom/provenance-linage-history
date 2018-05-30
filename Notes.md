# Feedback from @Davide

- Provenance section too wordy
-- break it up into more slides

- What's the difference between Linage & Provenance?
- P

# TODO

- Change Lineage to Succession
- Decide between Lineage and Provenance

- emphises the direction of traversal
-- forward => lineage
-- backward => provenance

- Fan Out vs Fan In
-- forward progression through processes much more likely to fan in
-- backward progression vice-versa

- Links between processes:
-- most often exist in the ancestor
-- like a linked list it is easier to traverse in a forward direction


- Implications are that:
-- it is naturally easier to do forward traversal => establishing lineage is easier
-- making backwards traversal easy requires planning; otherwise
-- requires high level knowledge of the production system
--- often looking up actions in a db from proir process groups

# Use more charts
Simple pipeline

(a) ──── (b) ──── (c) ──── (d)
───────── Succession ────────>
<──────── Provenance ─────────
<───────── Lineage ──────────>


Multiple input assets fan-in to produce a single output asset
         (b1) ─┐
(a1) ─┬─ (b2) ─┴─  (c1) ───  (d1)
(a2) ─┤
(a3) ─┘
───────── Succession ────────>
<──────── Provenance ─────────
<───────── Lineage ──────────>


Multiple input assets fan-in to produce a multiple output asset
(x1) ─── (b3) ─┬─  (y1) ───  (z1)
         (b1) ─┤
(a1) ─┬─ (b2) ─┴─  (c1) ───  (d1)
(a2) ─┤
(a3) ─┘
───────── Succession ────────>
<──────── Provenance ─────────
<───────── Lineage ──────────>


Where is this asset used?
- A question of Lineage

How was this asset produced
- A question of Provenance

Creating processes which record Lineage more natural for us to do.

