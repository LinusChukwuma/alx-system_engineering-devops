QUESTION


Using one of the web stack debugging project issue or an outage you have personally face, write a postmortem. Most of you will never have faced an outage, so just get creative and invent your own :)
Requirements:
•	Issue Summary (that is often what executives will read) must contain:
o	duration of the outage with start and end times (including timezone)
o	what was the impact (what service was down/slow? What were user experiencing? How many % of the users were affected?)
o	what was the root cause
•	Timeline (format bullet point, format: time - keep it short, 1 or 2 sentences) must contain:
o	when was the issue detected
o	how was the issue detected (monitoring alert, an engineer noticed something, a customer complained…)
o	actions taken (what parts of the system were investigated, what were the assumption on the root cause of the issue)
o	misleading investigation/debugging paths that were taken
o	which team/individuals was the incident escalated to
o	how the incident was resolved
•	Root cause and resolution must contain:
o	explain in detail what was causing the issue
o	explain in detail how the issue was fixed
•	Corrective and preventative measures must contain:
o	what are the things that can be improved/fixed (broadly speaking)
o	a list of tasks to address the issue (be very specific, like a TODO, example: patch Nginx server, add monitoring on server memory…)
•	Be brief and straight to the point, between 400 to 600 words
While postmortem format can vary, stick to this one so that you can get properly reviewed by your peers.
Please, remember that these blogs must be written in English to further your technical ability in a variety of settings.


ANSWER


Issue Summary: 
On February 5th, 2022 at 9:00 AM GMT, a web stack issue caused a 2-hour long outage that affected 75% of our users. During this time, users were unable to access the company's online store. The root cause of the issue was a software bug in the store's checkout page.
Timeline: 9:00 AM GMT on February 5th, 2022 - The issue was detected when a monitoring alert was triggered. The monitoring system detected a high number of error messages coming from the checkout page. 9:15 AM GMT on February 5th, 2022 - The issue was investigated by the IT Support Team. Assumptions were made that the root cause was a database connection problem, as the error messages suggested that there was a problem accessing the database. 9:30 AM GMT on February 5th, 2022 - Further investigation revealed that the issue was not related to the database connection, and the checkout page code was investigated instead. The Development Team was consulted and they found the software bug in the checkout page code. 10:00 AM GMT on February 5th, 2022 - The incident was escalated to the Development Team, who took ownership of the issue and worked on resolving it. 11:00 AM GMT on February 5th, 2022 - The incident was resolved by the Development Team by applying a software patch to fix the bug. The patch was thoroughly tested to ensure that the issue was fully resolved.
Root cause and resolution: The root cause of the issue was a software bug in the checkout page code. The bug caused the page to crash when a large number of users tried to access it at the same time. To resolve the issue, a software patch was applied to fix the bug. The patch was carefully reviewed to ensure that it didn't introduce any other problems and was thoroughly tested to confirm that it resolved the issue.
Corrective and preventative measures: To prevent similar incidents from happening in the future, the following measures will be taken:
•	Regular code reviews and testing to identify potential bugs before they cause problems. This will help ensure that the code is high-quality and free of bugs before it is released to the public.
•	Implementing automated testing to catch software bugs earlier in the development process. This will help identify potential bugs sooner and will reduce the risk of bugs causing problems in production.
•	Monitoring the checkout page performance more closely to detect potential issues sooner. This will allow the IT Support Team to identify problems earlier and take action before they escalate into outages.
•	Improving communication between the IT Support Team and the Development Team to ensure that incidents are handled more efficiently. This will reduce the time it takes to resolve incidents and will minimize the impact on users.

