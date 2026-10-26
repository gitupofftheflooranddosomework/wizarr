# CI cost policy

Never use paid GitHub Actions, GitHub-hosted runners (including free minutes),
larger runners, paid runner services, purchased minutes, or billing increases.
Use owned self-hosted runners or local validation only. Before pushing,
opening/updating a PR, dispatching or rerunning a workflow, inspect all workflows
and reusable workflows the action can trigger. Every executable job must use
an explicitly owned self-hosted runner. Unknown/dynamic routing fails closed.
If none is available, validate locally or leave CI blocked. Keep fork Actions
disabled. Existing hosted routing must be removed before triggering it.
