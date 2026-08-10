# RefuteGate validation history

This file records operational validation events for the synthetic sample study. It is not a
scientific result and does not change the study claims, protocol, measurements, or reported
results.

- On 2026-08-10, RefuteGate engine 0.5.0 at commit
  `e48b805b75065be9e2d224cba8c0ec4ff97f6a8f` reviewed source commit
  `f698ac44c4ce588e5e5914230d51225665a0790d` under job
  `c07499a3-01f8-4aea-8345-920f32d8ebb2`.
- That job published an operational failure receipt, not a scientific review result:
  `ERROR / CLAUDE_TIMEOUT / S2_ATTACK / provider_outcome=UNKNOWN`.
- Its preserved prefix contains an invalid Attack-claims response, one successful fresh-session
  claim repair, and a timed-out Attack-allegations call. No Coverage or Adjudication stage ran, so
  no scientific verdict or finding may be inferred from that job.
- RefuteGate 0.5.1 at commit `4401179b816189f1d887fefe82dde91f2504ee86`
  changes only the provider-specific structured-output transport and its verification contract:
  the supported Zhipu endpoint uses strict prompt-only JSON while Anthropic keeps native JSON
  Schema. The study evidence above remains unchanged.
