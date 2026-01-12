# GIS Team Workload Summary Prompt

## Purpose
Summarize the current workload for each GIS team member based on active M&D requests, highlighting work types, effort distribution, and key stakeholders.

## Context
You are analyzing GIS request data from Pilbara Ports Authority to provide a manager-level briefing on team capacity, work patterns, and demand sources.

## Input Format
You will receive M&D request data with the following fields:
- **Title** - Description of the request
- **Request Type** - Category of work
- **Status** - Current state (e.g., New, In Progress, Completed)
- **Assigned To** - GIS team member responsible
- **Requested By** - Person or team requesting the work
- **Business Unit** - Department making the request
- **Priority** - Urgency level
- **Due Date** - Target completion date
- **Description** - Detailed request information

## Task
Provide a plain-English summary for each team member (based on "Assigned To") that includes:

1. **What they're working on** - Brief overview of their active requests
2. **Nature of work** - Categorize as:
   - Ad hoc / Reactive
   - Repetitive / Maintenance
   - Decision-support / Strategic
3. **Effort level** - Indicate if workload is:
   - Light (1-2 requests)
   - Moderate (3-5 requests)
   - Heavy (6+ requests or multiple high-priority items)
4. **Demand sources** - Which business units or stakeholders are creating the most demand

## Output Format
Structure the summary as:

### [Team Member Name]
- **Current Focus:** [1-2 sentence summary of main work themes]
- **Work Type:** [Primary category with mix if applicable]
- **Workload Level:** [Light/Moderate/Heavy]
- **Priority Breakdown:** [Number of high/medium/low priority items]
- **Main Stakeholders:** [Top 2-3 requesters or business units]
- **Key Items:**
  - [Title] - Due: [Date] - Priority: [Level] - Requested by: [Name]
  - [Title] - Due: [Date] - Priority: [Level] - Requested by: [Name]
  - [etc.]

## Example Output
### Sarah Chen
- **Current Focus:** Supporting Operations and Planning teams with asset mapping and spatial analysis for port expansion
- **Work Type:** Decision-support / Strategic (70%), Ad hoc / Reactive (30%)
- **Workload Level:** Moderate
- **Priority Breakdown:** 2 High, 3 Medium, 1 Low
- **Main Stakeholders:** Planning & Development (3 requests), Operations (2 requests), Environment (1 request)
- **Key Items:**
  - Port infrastructure constraint mapping - Due: 15/02/2025 - Priority: High - Requested by: John Smith (Planning)
  - Asset condition spatial database update - Due: 28/02/2025 - Priority: Medium - Requested by: Maria Garcia (Operations)
  - Environmental buffer zone analysis - Due: 10/03/2025 - Priority: Medium - Requested by: David Lee (Environment)

---

## Additional Analysis (Optional)
If helpful, also provide:
- **Team-wide patterns:** Which business units are creating the most demand overall?
- **Capacity alerts:** Any team members with unusually high workloads or approaching deadlines?
- **Work balance:** Is the team focused more on strategic work or reactive requests?

## Notes
- Focus on requests with Status = "New" or "In Progress" (exclude "Completed" or "Cancelled")
- Keep descriptions concise and executive-friendly
- Avoid GIS jargon where possible
- Highlight business value, not technical implementation details
- Flag any high-priority items with approaching due dates
