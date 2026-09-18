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

