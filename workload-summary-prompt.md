# GIS Team Workload Summary Prompt

## Purpose
Summarize the current workload for each GIS team member based on active requests, highlighting work types and effort distribution.

## Context
You are analyzing GIS request data from Pilbara Ports Authority to provide a manager-level briefing on team capacity and work patterns.

## Input Format
You will receive a list of GIS requests with the following fields:
- Request description
- Request type
- Assigned team member
- Status
- Business area

## Task
Provide a plain-English summary for each team member that includes:

1. **What they're working on** - Brief description of their active requests
2. **Nature of work** - Categorize as:
   - Ad hoc / Reactive
   - Repetitive / Maintenance
   - Decision-support / Strategic
3. **Effort level** - Indicate if workload is:
   - Light (1-2 requests)
   - Moderate (3-5 requests)
   - Heavy (6+ requests or high-complexity items)

## Output Format
Structure the summary as:

### [Team Member Name]
- **Current Focus:** [1-2 sentence summary]
- **Work Type:** [Primary category]
- **Workload Level:** [Light/Moderate/Heavy]
- **Key Items:**
  - [Request 1 brief description]
  - [Request 2 brief description]
  - [etc.]

## Example Output
### Sarah Chen
- **Current Focus:** Supporting port expansion planning with constraint mapping and land use analysis
- **Work Type:** Decision-support / Strategic
- **Workload Level:** Moderate
- **Key Items:**
  - Port development constraint layer creation
  - Land use scenario mapping for Q2 planning
  - Environmental buffer zone analysis

---

## Notes
- Keep descriptions concise and executive-friendly
- Avoid GIS jargon
- Focus on business value, not technical tasks