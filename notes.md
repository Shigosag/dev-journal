### 1. docs: git cherry-pick note
Use 'git cherry-pick <hash>' to apply a specific commit to your current branch.

### 2. docs: git soft reset usage
'git reset --soft HEAD~1' unstages the latest commit while keeping file changes intact.

### 3. docs: git branch cleanup note
'git branch -d <name>' safely deletes locally merged branches.

### 4. docs: git stash with message
Use 'git stash push -m <msg>' to add clear context to stashed changes.

### 5. docs: git log oneline graph
'git log --oneline --graph --all' outputs a visual ASCII branch tree.

### 6. docs: docker prune dangling images
'docker image prune' removes untagged dangling images to reclaim disk space.

### 7. docs: docker tail container logs
Use 'docker logs -f --tail 100 <container>' to stream recent logs.

### 8. docs: docker compose up build flag
'docker compose up -d --build' rebuilds containers before launching in daemon mode.

### 9. docs: docker inspect ip address
'docker inspect -f {{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}} <container>' extracts IP.

### 10. docs: docker container stop timeout
'docker stop -t 30 <container>' gives tasks 30 seconds before sending SIGKILL.

### 11. docs: postgres explain analyze note
'EXPLAIN ANALYZE' executes the query and returns actual runtimes alongside the plan.

### 12. docs: postgres index selectivity note
B-tree indexes are most effective on columns with high cardinality.

### 13. docs: postgres connection pooling note
Use PgBouncer to manage high-frequency database connections efficiently.

### 14. docs: postgres jsonb containment note
Use the '@>' operator to query nested keys in PostgreSQL JSONB fields.

### 15. docs: postgres upsert conflict note
'ON CONFLICT (id) DO UPDATE' avoids duplicate key violations cleanly.

### 16. docs: linux find large files command
'find / -type f -size +100M' quickly locates large files consuming storage.

### 17. docs: linux check open ports note
'ss -tulpn' lists all listening TCP/UDP sockets with process IDs.

### 18. docs: linux tar archive shortcut
'tar -czvf archive.tar.gz /path' compresses directory using gzip.

### 19. docs: linux disk usage summary
'du -sh * | sort -h' shows human-readable disk usage per directory sorted.

### 20. docs: linux kill process by port note
'fuser -k 3000/tcp' kills the active process bound to port 3000.

### 21. docs: http status 429 rate limit
Status 429 indicates rate limiting; check 'Retry-After' response header.

### 22. docs: http idempotent methods note
GET, PUT, and DELETE are idempotent; POST and PATCH are typically non-idempotent.

### 23. docs: http cache-control directives
'no-cache' forces validation with origin server, whereas 'no-store' prevents caching entirely.

### 24. docs: http security headers note
Always configure 'Content-Security-Policy' and 'X-Content-Type-Options: nosniff'.

### 25. docs: http keep-alive benefits
HTTP keep-alive reuses existing TCP connections to reduce TLS handshake overhead.

### 26. docs: js promise allSettled note
'Promise.allSettled' handles multiple async operations without short-circuiting on error.

### 27. docs: js structured clone usage
'structuredClone()' provides a built-in deep copy mechanism for serializable objects.

### 28. docs: js optional chaining note
Optional chaining '?.' short-circuits gracefully when accessing null or undefined keys.

### 29. docs: js nullish coalescing note
Use '??' instead of '||' to preserve valid falsy values like 0 and false.

### 30. docs: js array flatMap method
'flatMap' maps elements and flattens the result by one level in a single pass.

### 31. docs: ts const assertions note
Using 'as const' creates deeply readonly object and tuple literals.

### 32. docs: ts utility type pick note
'Pick<T, K>' constructs a type by picking specific keys from an existing interface.

### 33. docs: ts utility type omit note
'Omit<T, K>' removes specified properties from a given type definition.

### 34. docs: ts unknown vs any note
'unknown' enforces type checking before operations, whereas 'any' disables safety.

### 35. docs: ts satisfies operator note
The 'satisfies' operator validates type compliance without widening literal types.

### 36. docs: react useId hook note
'useId' generates unique IDs for accessibility attributes across SSR and client.

### 37. docs: react memoization rule
Avoid premature optimization with 'useMemo'; profile renders before memoizing.

### 38. docs: react cleanup effect note
Always return a cleanup function in 'useEffect' for subscriptions and timers.

### 39. docs: react synthetic events note
React synthetic events wrap native events to provide cross-browser consistency.

### 40. docs: react fragments shortcut
Use '<>...</>' syntax to return multiple elements without adding extra DOM nodes.

### 41. docs: node event loop phases note
The Node.js event loop runs Timers, Pending Callbacks, Poll, Check, and Close phases.

### 42. docs: node stream backpressure note
Properly handle the 'drain' event to prevent memory bloat during file streams.

### 43. docs: node memory leak debug note
Use 'node --inspect' and Chrome DevTools heap snapshots to detect memory leaks.

### 44. docs: node cluster module note
The cluster module forks worker processes to utilize multi-core CPU architectures.

### 45. docs: node path resolve note
'path.resolve()' processes paths from right to left until an absolute path is resolved.

### 46. docs: css box-sizing border-box note
'box-sizing: border-box' includes padding and border within the specified width/height.

### 47. docs: css clamp function note
'clamp(min, preferred, max)' creates fluid responsive values without media queries.

### 48. docs: css flexbox gap property
The 'gap' property adds uniform spacing between flex items without margin hacks.

### 49. docs: css subgrid layout note
CSS subgrid allows nested grid items to inherit parent row and column tracks.

### 50. docs: css content-visibility note
'content-visibility: auto' skips rendering off-screen elements for faster page loads.

### 51. docs: bash script error handling
Use 'set -euo pipefail' at the top of bash scripts for strict error checking.

### 52. docs: bash command substitution note
Use '' instead of backticks for clean, nestable command substitution.

### 53. docs: bash parameter expansion
'default' provides fallback values for unset or empty shell variables.

### 54. docs: bash redirection note
'command > /dev/null 2>&1' silences both standard output and standard error.

### 55. docs: bash alias persistence
Store custom aliases in '~/.bashrc' or '~/.zshrc' to persist across terminal sessions.

### 56. docs: redis eviction policies note
'allkeys-lru' evicts least recently used keys when memory limits are reached.

### 57. docs: redis pub/sub pattern note
Redis Pub/Sub provides low-latency messaging but lacks message persistence.

### 58. docs: redis pipelining benefits
Pipelining bundles multiple commands to reduce round-trip network latency.

### 59. docs: redis hashes vs strings
Use Redis Hashes to store structured objects efficiently with less memory overhead.

### 60. docs: redis ttl command note
'EXPIRE key seconds' sets time-to-live for cache invalidation.

### 61. docs: nginx reverse proxy note
'proxy_pass http://localhost:3000' routes external requests to backend services.

### 62. docs: nginx gzip compression note
Enabling 'gzip_comp_level 5' balances CPU compression cost and bandwidth savings.

### 63. docs: nginx worker connections
Set 'worker_connections' based on system open file limits ('ulimit -n').

### 64. docs: nginx rate limiting zone
Use 'limit_req_zone' to protect sensitive authentication endpoints from brute force.

### 65. docs: nginx ssl termination note
Terminate SSL at Nginx to offload decryption overhead from backend applications.

### 66. docs: git interactive rebase note
'git rebase -i HEAD~N' allows squashing, renaming, and editing recent commits.

### 67. docs: git reflog recovery note
'git reflog' tracks all HEAD movements, enabling recovery of deleted branches.

### 68. docs: git worktree usage note
'git worktree add' lets you work on multiple branches simultaneously in separate folders.

### 69. docs: git shallow clone note
'git clone --depth 1' downloads only latest revision, speeding up CI pipeline checkout.

### 70. docs: git diff stat note
'git diff --stat' shows summary of modified files with inserted/deleted line counts.

### 71. docs: docker multi-stage build note
Multi-stage builds leave compiler toolchains behind, reducing image payload.

### 72. docs: docker non-root user note
Run applications as non-root user ('USER appuser') to enhance container security.

### 73. docs: docker healthcheck directive
Use 'HEALTHCHECK' in Dockerfile to allow orchestrators to detect deadlocks.

### 74. docs: docker buildkit cache note
Enable 'DOCKER_BUILDKIT=1' to leverage parallel step caching during builds.

### 75. docs: docker bridge network note
User-defined bridge networks allow containers to resolve each other by DNS name.

### 76. docs: sql foreign key cascade note
'ON DELETE CASCADE' automatically removes related child records when parent is deleted.

### 77. docs: sql window function note
'ROW_NUMBER() OVER (PARTITION BY group_id ORDER BY created_at DESC)' ranks grouped rows.

### 78. docs: sql join types note
INNER JOIN filters non-matching rows, while LEFT JOIN retains all rows from left table.

### 79. docs: sql cte benefits
Common Table Expressions ('WITH cte AS (...)') improve readability of complex subqueries.

### 80. docs: sql index on foreign keys
Indexing foreign key columns prevents full table locks during parent updates.

### 81. docs: curl timing metrics note
Use 'curl -w "%{time_total}" -o /dev/null -s <url>' to benchmark endpoint latency.

### 82. docs: curl follow redirects note
Pass '-L' to curl to automatically follow 301/302 HTTP redirect responses.

### 83. docs: curl pass auth header
Use 'curl -H "Authorization: Bearer <token>"' for bearer token authentication.

### 84. docs: curl send json payload
Use 'curl -X POST -H "Content-Type: application/json" -d '{"key":"val"}''.

