# Customizable Performance/Debug Overlay for Bevy UI

![docs](https://docs.rs/iyes_perf_ui/)
![MIT License](./LICENSE)

---

This crate provides an implementation of an in-game performance/debug UI overlay
for the [Bevy game engine](https://bevyengine.org).

```rust
commands.spawn(PerfUiCompleteBundle::default());
```

If you want to create a Perf UI with specific entries of your choice,
just spawn an entity with `PerfUiRoot` + your desired entries, instead
of using the bundle.

```rust
commands.spawn((
   PerfUiRoot::default(),
   PerfUiEntryFPS::default(),
   PerfUiEntryClock::default(),
   // ...
));
```
