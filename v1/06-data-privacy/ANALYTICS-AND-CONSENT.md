# Analytics and Consent

**Decision gate:** HD-002.

## Proposed default

METOYO 1.0 launches without third-party behavioral analytics.

The ritual must remain fully functional with analytics disabled.

## Allowed operational measurement candidate

If ratified, collect aggregate technical counters such as:
- ritual requests;
- successful responses;
- validation failures;
- model/source errors;
- coarse response latency bands;
- accessibility/system errors.

Do not attach:
- memory text;
- recipient identity;
- precise location;
- advertising IDs;
- cross-site identifiers;
- relationship profile.

## Product research

Prefer:
- opt-in usability studies;
- voluntary qualitative reflection;
- structured test cohorts;
- anonymous aggregate counters.

Do not turn Reflection into covert analytics.

## Consent separation

These are separate choices:
1. core processing necessary to answer the request;
2. optional save;
3. optional reflection;
4. optional research contribution;
5. optional product telemetry beyond strictly necessary operations.

One consent cannot silently authorize all five.

## Historical contradiction

Earlier project sources combine strict “no tracking / no cookies / no third-party analytics” claims with GA4, GTM, Bitly/UTM and Looker proposals.

METOYO 1.0 does not inherit both positions simultaneously.

Until HD-002 is ratified, production behavioral telemetry is OFF.

## Current platform note

If Supabase is used for persistence, all exposed tables require reviewed Row Level Security and explicit grants/policies. Production authorization is a database contract, not a UI assumption.
