# OpenSound dependencies

Application code: MIT, copyright OpenSound contributors. OpenSound code and fixtures are original; the following approved dependencies are licensed reuse. No DAW source code is reused.

| Direct dependency | License | Selection |
|-------------------|---------|-----------|
| Symphonia 0.5.5 | MPL-2.0 | Narrow WAV/PCM features, documented stable API. |
| Hound 3.5.1 | Apache-2.0 | Float WAV writer and independent test reader. |
| Rubato 0.16.2 | MIT | Fixed-ratio worker-side FFT conversion; delay/duration explicitly tested. |
| CPAL 0.16.0 | Apache-2.0 | WASAPI/device feasibility; not yet production-qualified. |
| serde / serde_json | MIT OR Apache-2.0 | Versioned project data. |
| anyhow | MIT OR Apache-2.0 | Control/worker error context. |
| sha2 | MIT OR Apache-2.0 | Content identity and integrity. |
| tempfile | MIT OR Apache-2.0 | Atomic file publishing. |
| uuid | MIT OR Apache-2.0 | Stable IDs. |
| clap | MIT OR Apache-2.0 | CLI parsing. |
| rtrb 0.3.2 | MIT OR Apache-2.0 | Bounded callback PCM/meter/capture queues. |
| Tauri 2 / dialog plugin | MIT OR Apache-2.0 | Native desktop shell and user-selected dialogs. |
| Tauri updater 2.13.3 | MIT OR Apache-2.0 | Signed, version-bound Windows updates through the official installer. |
| ebur128 0.1.10 | MIT | Standards-oriented loudness/true-peak analysis, histogram mode. |
| ctrlc | MIT OR Apache-2.0 | Explicit CLI cancellation/stop. |
| midly0.5.3 | Unlicense | Strict bounded SMF0/1 note interchange, std without parallel feature. |

Original DSP uses published W3C/RBJ biquad mathematics (attributed in the source register) and independently written dynamics/delay/reverb/limiter implementations. FunDSP was evaluated as a candidate but is not linked. Frontend runtime Tauri APIs are MIT OR Apache-2.0; Vite/TypeScript and their build dependencies need notices in the build inventory.

Pin documented DSP/device interfaces during initial feasibility; use Cargo.lock for all resolved versions. These are not claims that selected versions are latest. Upgrade deliberately after passing fixtures. Before distribution retain complete transitive license notices and corresponding source/license obligations; this initial inventory is not a finished redistribution audit.
