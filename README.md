# ClientModule

A Roblox client-side roll animation speed helper for local development and UI testing.

The helper keeps roll/result logic untouched. It exposes `_G.SafeRollSpeedScale` and
`_G.ApplyRollAnimationSpeed(configTable)` so your own animation code can shorten or
restore animation durations without changing luck, server-owned outcomes, paid-product
ownership, cooldowns, or other gameplay authority.

Configuration lives in `RollSpeedConfig` and is loaded with `require(script.RollSpeedConfig)`
so presets, default speed, minimum duration, and GUI labels can be adjusted without editing
the main helper script.
