# AI-Powered Personal Finance Assistant for College Students
Course: Fundamentals of MIS | SDG: Goal 10 — Reduced Inequalities


# The problem 
The problem is that San Jose parks and creek trails can have issues like illegal dumping, invasive plants, damaged trees, blocked trails, and erosion. These problems harm native plants, wildlife habitat, and public green spaces. The specific person affected is a San Jose park volunteer who notices these problems during a cleanup or trail walk. The failure point is that the volunteer may not know the right category, urgency level, environmental impact, or action needed. Since Milestone 1, the idea stayed mostly the same, but the system is now more focused on helping volunteers turn text reports and photos into clearer park maintenance reports.

The specific person affected is a San Jose park volunteer walking in a local park or along a creek trail. For example, the volunteer sees trash near a creek, overgrown plants blocking a trail, or damage near trees. They want to report it, but they do not know the right category, urgency level, or action needed.


# The AI capability 
My system uses two AI capabilities from the labs: structured data extraction and image recognition.

Lab 2 uses structured data extraction. This helps the system take a messy written report and turn it into clear fields. For example, a volunteer can write, “There is a large pile of trash near the creek trail.” The AI extracts the location, issue type, urgency level, environmental impact, and recommended action. This makes the report easier to review.

Lab 3 uses image recognition. This helps the system analyze a photo of a park or trail issue. The AI can identify visible problems like trash, blocked trails, damaged land, or overgrown vegetation. It can also explain possible risks and suggest what action should happen next. These two capabilities fit the project because volunteers often report problems with both words and photos.


# The workflow
The workflow starts when a San Jose park volunteer sees a problem in a park or creek trail. The volunteer either writes a short report, uploads a photo, or does both.

The AI then processes the input. If the input is text, the AI extracts structured fields such as location, issue type, urgency level, environmental impact, and recommended action. If the input is an image, the AI describes what is visible, identifies possible risks, and suggests a next step.

The output is a clearer park issue report. This report is not meant to make the final decision by itself. Park staff or trained volunteers should review the AI output first. If the output looks accurate, the report can be sent to the right service, such as cleanup, trail repair, tree assessment, invasive plant removal, or erosion control.


# Failure Case 
One failure case is when the system receives an input that does not fit the purpose of the AI Park Habitat Report Assistant. For example, I tested this prompt: “I'm having a really bad day. My cat knocked over my coffee and now my laptop isn't working. What should I do?”This input is not about a park, trail, habitat issue, or environmental damage. The system was designed for park reports, so this kind of personal technology problem is outside its purpose. The test was meant to see if the AI would force the message into the park report categories anyway.The AI handled this case well. It returned “N/A”, or “LOW” urgency_level. This shows the system did not create a fake park issue or send the report to park staff.Assessment: Acceptable. The system rejected an unrelated input correctly. However, this does not mean the system is safe in every case. A harder failure could happen with unclear photos or reports involving trash, personal belongings, or unhoused people. In those cases, the AI may label everything as illegal dumping when the situation needs human review.


# Oversight decision and the one change
A human should review the AI output before any real action happens. This is especially important when the report involves unclear photos, possible personal belongings, homelessness, safety risks, or multiple issue types. The AI can help organize the report, but it should not make final decisions that affect people or public spaces.

One change I would make is adding a “needs human review” flag. The system should use this flag when the AI is unsure, when the image is unclear, or when the issue may involve people’s belongings. This would help prevent the system from creating a harmful or wrong work order.

The tradeoff is that this slows down the process. More reports would need a person to check them before action happens. But this tradeoff is worth it because it reduces the chance of sending reports to the wrong department or harming people who are already vulnerable.
