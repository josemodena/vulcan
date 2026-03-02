# Language Support

## Tier 1 — Full Support

Full support means:
- Idiomatic output in the target language's style
- Complete mapping of all Dafny constructs to language equivalents
- Tests generated using the language's standard testing framework
- Inline proof annotations linked to verified Dafny methods

Python is the required default when no language is specified.

| Language |
|----------|
| **Python** |
| TypeScript |
| JavaScript |
| Rust |
| Go |
| Java |
| C |
| C++ |

## Tier 2 — Standard Support

Standard support means:
- Spec-to-code mapping for all Dafny constructs
- Best-effort idiomatic output (some constructs may be non-idiomatic)
- Tests generated; may require minor manual adjustment

| Language |
|----------|
| C# |
| Kotlin |
| Swift |
| Scala |
| Ruby |

## Tier 3 — Basic Support

Basic support means:
- Direct structural translation of Dafny constructs
- Minimal idiomatic adaptation
- All non-obvious constructs flagged for manual review in the diff

All languages not listed in Tier 1 or Tier 2 fall into Tier 3, **except Zig**.

## Explicitly Excluded

**Zig** is not supported at any tier.

## Requesting a Language

If your language is Tier 3 and the output is poor, open an issue describing
the specific Dafny constructs that didn't translate well. Tier promotions are
considered when there is a concrete spec-to-idiom mapping to implement.
