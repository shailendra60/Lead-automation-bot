# Lead-automation-bot
Automated Lead Intake &amp; Budget-Based Categorization System


**Project Title:** 
Automated Lead Intake & Budget-Based Categorization System

**Overview**
This project is an autonomous workflow built in n8n that automates the initial stages of the sales funnel. It is designed to capture potential customer data via a project lead form and provide instant categorization and notification, ensuring that high-priority leads are identified immediately without human intervention.

**Business Value & Problem** 
Solved Manual lead sorting is time-consuming and prone to delays. This automation solves these challenges by:
• Replacing "Human in the Loop": It eliminates the need for a person to manually check form submissions and notify the team.
• Vertical Scaling: It complements existing business workflows by handling repetitive administrative tasks, allowing team members to focus on high-value closing activities.

**Instant Prioritization**: By automatically labeling leads based on their project budget, the system ensures that "High Budget" opportunities are flagged for immediate follow-up.

**Key Features & Workflow Logic**
• Dynamic Intake: Uses an n8n Form trigger to collect essential lead data, including full name, project goals, timeframe, and budget.
• Intelligent Routing: Employs a Switch (Utility) Node to evaluate the "Project Budget" field and route the data through specific logic branches (Low, Medium, or High budget).
• Custom Notifications: Generates personalized email notifications via Gmail using dynamic expressions to map the lead's specific details into the subject line and body.
• Automated Gmail Labeling: Uses the Gmail API to dynamically apply color-coded labels (e.g., "High Budget Lead") to the email thread based on the routed path, allowing for an organized and visual inbox.

**Technical Stack**
• n8n: No-code workflow automation platform.
• Gmail API: For automated communication and thread management.
• JSON & Dynamic Expressions: For parsing and mapping data between nodes.
