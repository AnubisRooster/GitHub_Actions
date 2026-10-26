# Graph Report - GitHub_Actions  (2026-10-26)

## Corpus Check
- Corpus is ~12,507 words - fits in a single context window. You may not need a graph.

## Summary
- 44 nodes · 41 edges · 5 communities (4 shown, 1 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- steps
- auto-jira.yaml
- actions_settings_slackbalert.yaml
- steps

## God Nodes (most connected - your core abstractions)
1. `steps` - 6 edges
2. `steps` - 4 edges
3. `check-audit-log` - 3 edges
4. `send-webhook` - 3 edges
5. `env` - 3 edges
6. `schedule` - 2 edges
7. `jobs` - 2 edges
8. `issues` - 2 edges
9. `jobs` - 2 edges
10. `name` - 1 edges

## Surprising Connections (you probably didn't know these)
- None detected - all connections are within the same source files.

## Import Cycles
- None detected.

## Communities (5 total, 1 thin omitted)

### Community 1 - "steps"
Cohesion: 0.25
Nodes (8): runs-on, steps, check-audit-log, id, if, name, run, uses

### Community 2 - "auto-jira.yaml"
Cohesion: 0.25
Nodes (7): types, jobs, send-webhook, name, runs-on, True, issues

### Community 3 - "actions_settings_slackbalert.yaml"
Cohesion: 0.29
Nodes (6): jobs, name, cron, True, schedule, workflow_dispatch

### Community 4 - "steps"
Cohesion: 0.33
Nodes (6): JIRA_WEBHOOK_TOKEN, JIRA_WEBHOOK_URL, steps, env, name, run

## Knowledge Gaps
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `check-audit-log` connect `steps` to `actions_settings_slackbalert.yaml`?**
  _High betweenness centrality (0.061) - this node is a cross-community bridge._
- **Should `graphify_pipeline.py` be split into smaller, more focused modules?**
  _Cohesion score 0.13333333333333333 - nodes in this community are weakly interconnected._
- **Why does `jobs` connect `actions_settings_slackbalert.yaml` to `steps`?**
  _High betweenness centrality (0.053) - this node is a cross-community bridge._