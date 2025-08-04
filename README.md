# Deno pnpm compat issue

Problem: You can never introduce a deno app into an existing pnpm workspace without either:

1. Treating the deno workspace member as an isolated project (no dependency sharing with other workspace members, might lead to duplicated peer deps)
2. Convert everything to Deno workspaces.
