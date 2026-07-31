# Praesenta attestation anchors

Nightly sha256 commitments to Praesenta Research's append-only,
hash-chained ledger of published model states.

Each line in `anchors.log` (and file under `anchors/`) commits to
the full ledger as of that session: its line count and the sha256
of its final hash-chained line. `.ots` files are OpenTimestamps
proofs anchoring the same statements into Bitcoin.

The ledger itself is private until launch. When published, anyone
can verify that every line existed — unaltered — on the date its
anchor was committed here: recompute the hash chain, compare tails.
A commitment posted here cannot be rewritten to fit later data;
that is the point.
