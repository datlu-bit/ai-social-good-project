# AI-Powered Personal Finance Assistant for College Students
Course: Fundamentals of MIS | SDG: Goal 10 — Reduced Inequalities


# The problem 
The problem is that San Jose parks and creek trails can have issues like illegal dumping, invasive plants, damaged trees, blocked trails, and erosion. These problems harm native plants, wildlife habitat, and public green spaces. The specific person affected is a San Jose park volunteer who notices these problems during a cleanup or trail walk. The failure point is that the volunteer may not know the right category, urgency level, environmental impact, or action needed. Since Milestone 1, the idea stayed mostly the same, but the system is now more focused on helping volunteers turn text reports and photos into clearer park maintenance reports.

The specific person affected is a San Jose park volunteer walking in a local park or along a creek trail. For example, the volunteer sees trash near a creek, overgrown plants blocking a trail, or damage near trees. They want to report it, but they do not know the right category, urgency level, or action needed.


# The AI capability 
First, it uses structured data extraction from Lab 2. This helps turn a messy written report into clear fields like location, issue type, urgency level, environmental impact, and recommended action.

Second, it uses image recognition from Lab 3. This helps analyze a photo of a park issue and identify what problem is visible, how serious it looks, and what action may be needed.

These capabilities fit the problem because park volunteers often report issues using both written descriptions and photos.


# The workflow
Input: A park volunteer submits a written report or uploads a photo of a park issue.

AI step: The AI reads the text or analyzes the image. It identifies the location, issue type, urgency level, environmental impact, and recommended action.

Output: The AI creates a clearer report for park staff.

Real-world action: Park staff or trained volunteers review the AI output. If the report is accurate, they send it to the right service, such as cleanup, trail repair, tree assessment, invasive plant removal, or erosion control.


# Failure Case 
One failure case is when the AI sees a photo with trash and personal belongings near trees or a trail. The system may label everything as illegal dumping. But some items may belong to an unhoused person. If the AI creates a cleanup order without human review, someone’s belongings could be removed without proper support.

This failure is possible because the image alone cannot always explain the full situation. The AI can identify visible objects, but it cannot fully understand the human context.


# Oversight decision and the one change
A human should review the AI output before any real action happens, especially for sensitive cases. This includes reports involving homelessness, personal belongings, unclear images, safety risks, or mixed categories.

One change we would make is adding a “needs human review” flag. The system should flag reports when it sees possible personal belongings, unclear evidence, or multiple issue types.

The tradeoff is that this slows down the process. More reports need human review, so the system is less automated. But it reduces the chance of harming people or sending reports to the wrong department.
