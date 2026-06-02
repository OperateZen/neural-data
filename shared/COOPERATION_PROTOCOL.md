# OperateZen Agent Cooperation Protocol v1.0

## How Agents Work Together

### Create → Broadcast → React
1. Any agent creates data (lead, ticket, client, etc.)
2. Auto-broadcasts to ALL agents via AgentMessage
3. Relevant agent responds (e.g. Zara sends welcome email for new lead)

### Query → Discuss → Trigger
1. Sierra queries Lead data → sees 5 new leads
2. Posts discussion: "Zara — send welcome emails?"
3. Can optionally auto-trigger Zara's action

### Search → Improve → Learn
1. Agent searches GitHub + platform for a pattern
2. Finds issues, logs improvements to KnowledgeBase
3. Never creates duplicate entries (fingerprinted by agent + first 80 chars)

### Crypton Provisions
1. Crypton creates team members as "helpers"
2. Each helper gets tasks auto-assigned
3. Announced to all agents, synced to neural-data repo

## API Endpoint
POST https://itmanage-hub-479bc828.base44.app/api/functions/ozAgentAPI
Header: api_key: f3c87607c72d4e9c9bdeae80265cbd54

## Actions
| action | description |
|---|---|
| agent_action | Universal: create client/lead/password/checklist/task/backup/member |
| agent_discuss | Agent→Agent discussion + optional trigger chain |
| agent_query | Query platform data + auto-generate discussion |
| agent_search | Search GitHub + platform for fixes/improvements |
| agent_improve | Scan platform, find issues, log improvements |
| crypton_provision | Crypton creates helper agents + assigns tasks |
| backup | Full platform backup to neural-data repo |

## Data Sources
- Live platform: https://itmanage-hub-479bc828.base44.app
- GitHub test data: OperateZen/operatezen_beta
- Neural data: OperateZen/neural-data (this repo)
