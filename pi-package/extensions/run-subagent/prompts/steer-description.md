DESCRIPTION: Send a follow-up prompt to a previously started child session.

USAGE:
1. A single continuation call is valid.
2. Use `subagent_steer` only to adjust an active invocation or continue a terminal session within the same atomic task.
3. Include only changed requirements, decisions, findings, acceptance criteria, or evidence needed for the continuation.
4. Use `subagent_start` for an independent task or a different specialist.
5. Write the follow-up prompt in ASD-STE100 Simplified Technical English.

CONSTRAINTS:
1. Do not reuse one session for multiple subtasks.
2. Do not steer a running child merely to request status or push it to finish. Use automatically delivered feedback or `subagent_wait`.
