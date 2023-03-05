Issue Summary:
Duration: 1 hour, from 2:00 PM to 3:00 PM GMT+1
Impact: Backend API was down resulting in all services dependent on it being inaccessible. Users were unable to perform actions on the app, and all services were showing errors. Approximately 90% of users were affected.

Timeline:

2:00 PM: Issue detected through monitoring alert.
2:05 PM: Investigation began on the backend servers and logs were analyzed for the root cause.
2:15 PM: Debugging revealed that the error was being caused by a database connection issue.
2:30 PM: Investigation focused on the database servers and logs were analyzed for the root cause.
2:45 PM: It was discovered that the database server had run out of disk space causing the database to fail.
2:50 PM: The incident was escalated to the database team for immediate resolution.
3:00 PM: The incident was resolved, and the backend API service was restored.
Root cause and resolution:
The root cause of the issue was determined to be the database server running out of disk space, causing the database to fail. The database team resolved the issue by freeing up disk space, and the database server was brought back up. Once the database server was functional, the backend API was automatically restored.

Corrective and preventative measures:

Implement automatic monitoring and alerting systems for disk space usage.
Implement a system to automatically scale up database servers when disk space usage is getting low.
Increase the size of the database server disks to accommodate growth.
Create a backup system for the database server to prevent data loss in case of disk failure.
Develop a response plan to quickly address database server issues when they occur.
Overall, we apologize for the inconvenience caused to our users. We have taken necessary steps to prevent this issue from happening again in the future. We will continue to monitor our systems and improve our infrastructure to ensure that our services are always available to our users.
