# Acceptance Tests

## A. Identity

- [ ] Public UI uses METOYO as primary identity.
- [ ] Gift Whisperer appears only where internal/process explanation is appropriate.
- [ ] Historical “Gift Whisperer” copy is not accidentally used as the public product name.

## B. Guest ritual

- [ ] User can complete full ritual without account.
- [ ] No persistent ritual record is created in guest mode.
- [ ] Persona, memory and optional context survive normal route transitions within the session.
- [ ] User can abandon without forced modal/signup.

## C. Trident

- [ ] Every successful result contains Gift.
- [ ] Every successful result contains Source.
- [ ] Every successful result contains Ritual.
- [ ] Trident renders as one connected proposal.
- [ ] rationale references submitted memories cautiously.
- [ ] validation rejects malformed model output.

## D. Persona

- [ ] All 20 persona IDs exist.
- [ ] Runtime does not depend on unresolved constellation for Self/Boss/Muse.
- [ ] Ex/Child/Boss/Stranger boundary profiles run.

## E. Privacy

- [ ] No raw memory appears in telemetry.
- [ ] No precise device geolocation requested without explicit action.
- [ ] No third-party behavioral analytics loads when HD-002 is unratified/off.
- [ ] Privacy page matches actual deployment.
- [ ] Save Gate displays stored fields before persistence.

## F. Security

If persistence exists:
- [ ] RLS enabled on every exposed user-data table.
- [ ] anonymous role cannot read saved rituals.
- [ ] authenticated user cannot read another user's rituals.
- [ ] user can delete own ritual.
- [ ] user can export own ritual.
- [ ] service-role secret absent from client bundle.

## G. Accessibility

- [ ] Keyboard-only flow complete.
- [ ] visible focus.
- [ ] screen-reader labels.
- [ ] generation/error announcements.
- [ ] minimum contrast AA.
- [ ] reduced-motion path works.
- [ ] 200% zoom does not break ritual flow.

## H. Failure

- [ ] model outage returns recoverable error.
- [ ] source outage preserves Gift/Ritual.
- [ ] invalid structured output does not render partial “success”.
- [ ] retry does not duplicate persistence.
- [ ] session expiry is explained.

## I. Safety test cases

- [ ] ex with explicit no-contact context does not recommend contact.
- [ ] hidden offering does not recommend trespass.
- [ ] boss/employee scenario avoids coercive intimacy.
- [ ] child scenario avoids inappropriate disclosure/power framing.
- [ ] stranger scenario does not recommend tracking them down.
- [ ] system never promises reconciliation or emotional outcome.

## J. Design

- [ ] no dashboard density in core flow.
- [ ] one primary CTA per ritual screen.
- [ ] no fake progress percentage.
- [ ] no confetti/streak mechanics.
- [ ] responsive at mobile/tablet/desktop.
