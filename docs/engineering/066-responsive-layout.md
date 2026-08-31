# Responsive Layout

## Purpose

Define a clear, testable responsive layout standard for ColorSense so future changes preserve predictable game behavior and remain easy to review.

## Required outcome

The responsive layout rules must work with the existing dependency-free browser game, cover failure and fallback behavior, and avoid unrelated changes.

## Acceptance criteria

- The responsive layout behavior is explicit and observable.
- Easy and Hard modes continue to work.
- Keyboard, touch, and assistive-technology impact is considered.
- Verification requires no private service or production credential.
- User-facing changes include before-and-after evidence.

## Verification checklist

- [ ] Exercise Easy and Hard modes.
- [ ] Check mobile and desktop viewport sizes.
- [ ] Confirm reset and replay behavior.
- [ ] Confirm the browser console has no new errors.
- [ ] Record unrelated follow-up work separately.

## Review guidance

Keep the implementation focused on one responsive layout outcome. Document migration, compatibility, privacy, or rollback impact whenever applicable.