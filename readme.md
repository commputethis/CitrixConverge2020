# Team OPEF

IT Operational Efficiencies using Microapps + Ansible Tower + Powershell + GitLab to streamline and consolidate tools and systems with one front end.

## Team members

- Jeremy Becker
- [Devan Tilly](https://twitter.com/devantilly)
- [David Prows](https://twitter.com/commputethis)

## For the Hackathon presentation

### How we came about the idea

In the past year our company has been in a devops revolution, we have setup GitLab and Ansible Tower to design and implement scripts that handle mundane, and tedious tasks. With Microapps we were able to create a one stop shop for not only our devops needs, but the needs of our frontline staff. Microapps integrations will enable our staff to provide business continuity and growth. Now that we have an understanding of how Microapps work, we will be adding additional tools for devops, business continuity and to make our frontline staff’s jobs more efficient.

### What we have learned

- Learned some basics of JSON
- Fundamental knowledge of REST APIs
- How pagination combined with queries can be used to create a table with only the latest result
- How to use and setup webhooks
- Basic understanding of using Private and Foreign keys in Tables
- We learned how to use Postman to test our API calls

### What challenges we faced

- Ran into SSL cert issues where intermediate CA certs were missing. We overcame this by uploading the full certificate bundle to the server.
- Ran into issue where Citrix RSS Feeds template does not support on-prem feeds. We may look at creating our own microapp for this vs using the template.
- Having issues with communicating with the DUO Security API.  We haven't overcome this yet, but will keep working on it.
- Lack of knowledge of webhooks, Microapps UI, and REST APIs.  We overcame this by reading a lot of documentation and watching some youtube videos.

## Project Scope

Utilize Microapps to Prevent System Outages, Guard Against Security Breaches, Manage System Upgrades, and help with Business Continuity.

## What we would like to do

### Phase 1

- Integrate with Ansible Tower and add common job templates (Completed)
  - AD SAM Uncheck (Completed)
    - With more employees transitioning to work from home, we have had more and more instances of users not being able to change their expired passwords, and when this happens our Frontline staff do not have the permissions to uncheck the “User must change password at next logon” box in AD. Which causes undue stress on both the end user and the frontline staff that are following the security policies. Integrating a Tower job into MicroApps we were able to give our frontline staff the ability to uncheck the box without giving their accounts the necessary permissions, and streamlining the process at the same time.
  - Machine Catalog Update (Completed)
    - Utilizing Microapps we were able to streamline the process of updating machine catalogs, that have had Windows Updates or some other software upgrade installed. Enabling us to update multiple machines catalogs with new images, without having to sign into Citrix cloud studio.
  - Maintenance Mode Timed (Completed)
    - In the past our staff has accidentally caused degraded performance or potential outages, by leaving Citrix machines in maintenance mode for too long. To prevent these potential outages we designed a script that takes the machines to be placed in maintenance mode and the allotted time and removes them after the time expires.

### Phase 2

- Integrate with GitLab (Completed)
  - Merge Request Approval (Completed)
    - We utilize Gitlab to create, increment and update scripts, as well as for documentation. One annoyance we have come across is when we merge branches, we prefer that another staff members reviews and approves the merge requests, which requires signing into Gitlab, and then navigating through various menus. With Microapps we were able to provide a notification for when a merge request was placed and then anyone on our team would then be able to review the merge request, and approve it without ever having to sign into Gitlab.
- Further Integrate with Ansible Tower
  - Additional Job Templates that are used by Staff
- Integrate with DUO
  - Unlock users

### Phase 3

- Integrate with Solarwinds Orion
  - Pull bandwidth usage for remote offices
  - Receive notifications of trouble
- Integrate with Splunk
  - Run queries and pull back results
- Integrate with our Help Desk Ticketing system
- Integrate other systems as needed

## Recommended References

- Citrix Developer Site - [https://developer.cloud.com/](https://developer.cloud.com/citrixworkspace/citrix-workspace-platform/build-workspace-microapp-integrations/docs/overview)
- GitLab Docs - [https://docs.gitlab.com](https://docs.gitlab.com/ee/api/README.html)
- Ansible Tower Docs - [https://docs.ansible.com](https://docs.gitlab.com/ee/api/README.html)
- How to create a Basic Citrix Microapp - [https://www.youtube.com](https://youtu.be/qdwuZQRd1Lg)

### Overall, learned something new, had fun, and expanded our codeverse(tm)
