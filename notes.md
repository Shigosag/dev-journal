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

