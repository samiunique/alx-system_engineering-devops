https://medium.com/@yitesam/postmortem-server-outage-due-to-code-bug-and-mis-7f54e642d452
<br>


Postmortem: Server Outage Due to Code Bug and Misconfiguration<br>
<br>
Issue Summary
- Duration:
— Start Time: 03, 14, 2024, 10:00 AM UTC.
— End Time: 03, 14, 2024, 12:30 PM UTC.
- Impact:
— The outage significantly impacted our web application’s availability, resulting in a 30% decrease in user engagement during the downtime.

Timeline
1. 10:00 AM UTC: Reports of issues start arriving.
2. 10:15 AM UTC: DevOps team alerted and begins investigation.
3. 10:30 AM UTC: Server returns “HTTP 500 Internal Server Error” responses.
4. 10:45 AM UTC: Debugging tools deployed for root cause analysis.
5. 11:00 AM UTC: Issue traced to misconfigured database connection pool.
6. 11:15 AM UTC: Culprit identified: misconfigured database connection pool.
7. 11:30 AM UTC: Fix implemented by adjusting connection pool settings.
8. 11:45 AM UTC: Corrected code deployed to the server.
9. 12:00 PM UTC: Situation monitored for stability.
10.12:30 PM UTC: Service fully restored.

Root Cause
- Recent code changes led to inadvertent modification of the database connection pool configuration, resulting in exhausted database connections and server failure.
<br>
 <a href="https://imgur.com/pt6OpA9"><img src="https://i.imgur.com/pt6OpA9.gif" title="source: imgur.com" /></a>
<br>
Resolution and Recovery
- DevOps team swiftly identified and adjusted the misconfiguration.
- Thorough testing conducted using “curl” to ensure correct server response.
- Corrected code deployed, restoring server functionality.

Corrective and Preventative Measures
1. Automated Testing:
— Implement automated tests to catch configuration issues during deployment.
— Regularly validate database connections to prevent similar incidents.

2. Code Reviews:
— Enforce thorough code reviews to catch misconfigurations early.
— Scrutinize changes to critical components like connection pools.

3. Documentation and Runbooks:
— Maintain clear documentation on server configurations and dependencies.
— Create runbooks for troubleshooting common issues.

4. Monitoring and Alerts:
— Set up proactive monitoring for critical services.
— Configure alerts to notify the team promptly of anomalies.

5. Training and Awareness:
— Conduct periodic training sessions to reinforce best practices.
— Remind developers of the importance of configuration management.
