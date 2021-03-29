# chatstats

### API HOW TO CALL

https://api.slack.com/web#basics 

## As the ChatStats app user, I want to:

### Phase 1:
Confirm OAuth behind the scenes -- app is installed with permissioning and does not need to be validated afterward

Be invited to a channel

### PHASE 1 API CALLS

OAuth Join: https://api.slack.com/authentication/oauth-v2 
Join a conversation by ID: https://api.slack.com/methods/conversations.join

### Phase 2: 
When called, react with: 
- Grab room name 
- Grabbing user info and user email
- Grabbing link to message

### PHASE 2 API CALLS

Search within threads: https://api.slack.com/messaging/retrieving#finding_threads

Retrieve payload: https://api.slack.com/messaging/retrieving 

### Phase 3:
Posting in #chatstats channel:
“New CSS interaction found: “
- Post user name 
- Post user email 
- Post Room Name 
- Post link to the message

### PHASE 3 API CALLS

Join another room: https://api.slack.com/methods/conversations.join

Retrieve message from last room: https://api.slack.com/methods/conversations.history

Post a message in new room: https://api.slack.com/methods/chat.postMessage 

### FUTURE STATE: 
- Counting number of posts? 
- Limit by date range? 
- Emoji react? Workflow builder + Custom app step
- Be invited to 3 channels 
