---
title: approval required for {{ env.ENVIRONMENT }}
labels: approval-requested
---
approval requested from {{ payload.sender.login }}.
Comment "approved" to kick project.

'''json target_payload
{
    "runNumber": {{ env.RUNNUMBER }},
    "environment": "{{ env.ENVIRONMENT }}"
}
'''
