Issue Summary:
On March 1st, 2023 from 2:30 PM to 3:15 PM WAT, users were unable to access the backend API service, resulting in a 500 error. Approximately 30% of users were impacted during this time. The root cause was identified as a database connection issue.

Timeline:

2:30 PM: The issue was detected by monitoring alerts.
2:32 PM: An engineer was notified and began investigating the issue.
2:40 PM: Investigation showed that the backend API was returning a 500 error and the root cause was suspected to be a database connection issue.
2:50 PM: Misleading investigation paths were taken, including checking server logs and restarting the API service.
3:00 PM: The incident was escalated to the database team for further investigation.
3:15 PM: The database team identified the issue as a misconfiguration in the database connection pool and corrected the configuration.
3:20 PM: The backend API service was restored to normal functionality.
Root Cause and Resolution:
The root cause of the issue was a misconfiguration in the database connection pool, which led to the backend API service being unable to establish connections to the database. The database team corrected the configuration and tested the service to ensure it was functioning properly.

Corrective and Preventative Measures:
To prevent similar issues from occurring in the future, the following corrective and preventative measures will be taken:

A post-incident review will be conducted to identify any gaps in monitoring and alerting.
The database connection pool configuration will be reviewed and updated to ensure proper connection handling.
Additional logging and monitoring will be implemented to provide greater visibility into database connection issues..
