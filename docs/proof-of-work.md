# Projects

Practical artifacts from 18 years of delivery: templates, plans and tools I use and share.

## Application decommissioning

Artifacts from a five-year programme that retired 500+ legacy applications.

<div class="grid cards" markdown>

- **Application Inventory Template**

    The analysis-phase workbook: one row per application, capturing owner, usage, cost, business capability, data retention needs and the retire / archive / retain decision.

    [Download app inventory and IT portfolio analysis template (.xlsx)](https://github.com/nilabh-sharma/PM_Templates/raw/main/XXXXX_Application_Inventory_Template_decommission.xlsx){ .md-button }

- **Monthly Status Deck**

    Monthly steering committee template: overall RAG, delivery and savings KPIs, wave pipeline, risks and decisions needed.

    [Download sample monthly slide (.ppt)](https://github.com/nilabh-sharma/PM_Templates/raw/main/AMS_Decommissioning_May2021.pptx){ .md-button }

</div>

## AI adoption strategy and planning

A 90-day programme taking five delivery teams from AI awareness to AI agents in daily use.

<div class="grid cards" markdown>

- **90-Day AI Adoption Programme**

    Phased plan (enable, build, adopt), team rollout, success metrics and governance for GitHub Copilot, Glean and Databricks Genie.

    [Download AI adoption plan template (.xlsx)](https://github.com/nilabh-sharma/AI-Plan-agent/raw/main/AI_ADOPTION_ROADMAP_TRACKER.xlsx){ .md-button }

 - **AI Agent Demo: Jira ticket to schema change**

    A working agent that picks up a Jira ticket requesting a table change (DDL), makes the change, and updates the ticket with what it did, with no manual hand-offs between the steps.

    1. Reads the ticket and works out the required schema change
    2. Generates and applies the DDL update
    3. Comments on the ticket with the change made
    4. Moves the ticket to the next status

    <video controls preload="metadata" style="width:100%; border-radius:8px;">
      <source src="https://github.com/nilabh-sharma/AI-Plan-agent/raw/main/AI_AGENT_WORKING_DDL_UPDATE%20%281%29.mp4" type="video/mp4">
    </video>

    [Watch on GitHub](https://github.com/nilabh-sharma/AI-Plan-agent/raw/main/AI_AGENT_WORKING_DDL_UPDATE%20%281%29.mp4){ .md-button }

</div>

## Customer journey analytics: data delivery plan

Delivering 50 customer insight attributes for Customer Journey Analytics on Databricks in eight weeks, with one attribute group dependent on a third-party data feed. The challenge was planning work that could not wait for requirements to be finished, and protecting the go-live date from a supplier I did not control.

<div class="grid cards" markdown>
- **Project Plan & Delivery Tracker**

    An eight-week plan that runs requirements, data analysis, design and build in overlapping attribute batches, so work on well-understood attributes starts while others are still being defined.

    - **Gantt:** phases, dependencies and gates, driven by a single start date
    - **Third-party track:** the supplier feed as its own critical-path swimlane, with a week-4 fallback decision
    - **Attribute tracker:** all 50 attributes, from definition to UAT sign-off
    - **Milestones & RAID log:** gates, risks, assumptions and dependencies

    [Download the plan (.xlsx)](https://github.com/nilabh-sharma/PM_Templates/blob/main/CJA_Customer_Insight_Views_Project_Plan_NS.xlsx){ .md-button }

</div>


## Snowflake vs. AWS Redshift: a warehouse platform evaluation

Picking a cloud warehouse on feature lists is easy. Knowing what it will cost to run and operate is the hard part. This evaluation puts the two platforms side by side on architecture, how much operational work each needs, and costed estimates for production, development and test, so the decision rests on total cost of ownership rather than list price.

<div class="grid cards" markdown>

- **Outcome**

    Snowflake was selected. Separating compute from storage, scaling without downtime and needing less tuning work gave it a lower estimated annual cost for the same workloads.

    [Download Snowflake vs AWS Redshift evaluation deck (.pptx)](https://github.com/nilabh-sharma/PM_Templates/raw/main/Snowflake%20%26%20AWS%20Redshift%20Evaluation_Comparison.pptx){ .md-button }

</div>

---

[All PM templates on GitHub](https://github.com/nilabh-sharma/PM_Templates){ .md-button }
