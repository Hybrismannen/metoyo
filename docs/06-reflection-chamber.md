# 06 — Reflection Chamber

## 1. Purpose

Most digital systems treat completion as the end of a transaction.

METOYO treats the moment after the gesture as potentially meaningful, but not as an opportunity to harvest engagement.

The **Reflection Chamber** is an optional, private space for noticing what happened after the gift or gesture entered the world.

## 2. Entry

After a Trident is generated, the user may be asked:

> **Would you like to return to this gesture later?**

The answer may be:
- no;
- yes, at a user-selected time;
- yes, using a suggested light interval.

Historical planning suggested **3–7 days** after the gesture, but that interval is not a mandatory product rule.

## 3. Reflection prompts

Possible prompts include:
- What happened when you gave it?
- What stayed with you afterward?
- What did you notice in yourself?
- Was there a silence that mattered?
- Did the gesture feel proportionate?
- Would you give differently next time?
- What did you remember that you had not expected to remember?

Prompts should not:
- interpret another person's reaction;
- push for disclosure;
- demand a positive outcome;
- measure emotional performance;
- imply therapeutic processing.

## 4. Reflection is not feedback

The Chamber is distinct from:
- NPS;
- star ratings;
- product satisfaction;
- conversion surveys;
- retention mechanics;
- social proof collection.

A user may choose to provide separate voluntary project feedback, but that must not be confused with their private reflection.

## 5. Data model

Default:

```yaml
reflection:
  enabled: false
  storage: none
  analytics: none
```

If the user explicitly chooses to save:

```yaml
reflection:
  enabled: true
  owner: user
  exportable: true
  deletable: true
  analytics: off_by_default
  public_sharing: separate_opt_in
```

## 6. User sovereignty

If persistence exists, the user should be able to:
- keep the reflection private;
- export it;
- delete it;
- decline future reminders;
- save only selected entries;
- avoid account creation where technically possible.

## 7. Ritual Wall distinction

Historical planning included an optional **Ritual Wall**: a public gallery of anonymized gifting moments.

The Ritual Wall, if ever implemented, is a separate module.

It must require:
- explicit submission;
- clear consent for publication;
- review for identifying details;
- no automatic migration from private reflection;
- no assumption that anonymity is guaranteed merely by removing names;
- withdrawal/removal mechanism.

## 8. Success logic

The Reflection Chamber succeeds when it helps a user integrate a gesture.

It is **not** successful merely because:
- many users return;
- entries are long;
- people share emotionally intense stories;
- public submissions grow.

A decline in system dependence may be a stronger success signal than repeated journaling.

## 9. Tone

The Chamber should feel:
- quiet;
- optional;
- non-analytic;
- unhurried;
- non-performative.

Avoid:
- badges;
- streaks;
- "you haven't reflected yet";
- sentiment scores;
- automated psychological interpretations;
- public comparison.

## 10. Core principle

> Reflection belongs to the person before it belongs to the project.

The system may offer a place to notice. It should not convert that noticing into extractive data.
