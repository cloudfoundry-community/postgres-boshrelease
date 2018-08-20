# Improvements

In this release we've fixed a bug where keepalived was disabled, no matter the
setting. The intended logic of "keepalived is enabled by default, disabled via
`keepalived.enabled: false`" holds.
