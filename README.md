Data Privacy Policy for Zenial System, Zenial Admin, Zenial Voice and Zenial Ticket
These services are jointly referred to as Zenial Bots in this policy.

Effective date: February 16, 2026
Policy version: 1.0

1. Scope
This policy explains how Zenial Bots process personal data when used in Discord servers.

2. Controller and Contact
Controller: Zenial Network / Zenial Bot Operator
Contact email: privacy@zenial.example (replace with your real address)
Discord contact: Zenial support team (replace with your official support contact)

3. Services Covered
Zenial System
Zenial Admin
Zenial Voice
Zenial Ticket

4. Data We Process
Zenial Bots may process:
Discord identifiers such as user ID, guild ID, channel ID, role ID, message ID and interaction IDs
Account and member context such as usernames, display names, role memberships, permissions, and join/leave and moderation context
Message data used by enabled features, including message content, attachments, sticker metadata, embeds, links and message references
Voice state data, including channel joins/leaves/switches, ownership of temp voice channels, and channel membership lists
Ticket data, including creator, assigned supporter, participants, status, ticket counters, transcript metadata and transcript files
Operational telemetry such as command usage entries, timestamps, internal logs and error logs

5. Intent and Feature Review
The following review is based on the current bot code in this workspace.

Zenial System
Configured intents: Guilds, GuildMembers, GuildMessages, DirectMessages, GuildVoiceStates, MessageContent
MessageContent is required for chat EXP, global chat relay, invite detection in global chat and Pokemon answer checks.
GuildMembers is required for member fetches, role operations, permission checks and guild join validation.
GuildVoiceStates is required for periodic voice EXP calculation from current voice states.
GuildMessages is required for message create/update/delete/bulk handlers.
Guilds is required for slash commands and guild lifecycle handlers.
DirectMessages is configured; no dedicated DM message handler is currently present.

Zenial Admin
Configured intents: Guilds, GuildMembers, GuildMessages, DirectMessages, GuildVoiceStates, MessageContent
MessageContent is required for moderation message analysis, autoscam scoring, message logs and custom text commands.
GuildMembers is required for join/leave/update events, moderation role actions, invite tracking and member fetches.
GuildVoiceStates is required for voice-state moderation rules.
GuildMessages is required for message create/update/delete/bulk logging and moderation.
Guilds is required for command handling and guild lifecycle logic.
DirectMessages is configured; no dedicated DM message handler is currently present.

Zenial Voice
Configured intents: Guilds, GuildMembers, GuildVoiceStates
GuildVoiceStates is required for auto-creation/cleanup of temporary voice channels and ownership transfer logic.
GuildMembers is required for ownership checks, immune-role checks, member fetches and permission updates.
Guilds is required for slash commands, interaction handling and guild lifecycle checks.

Zenial Ticket
Configured intents: Guilds, GuildMembers, GuildMessages, DirectMessages, GuildVoiceStates, MessageContent
MessageContent is required for support-trigger checks and message handling in ticket channels.
GuildMessages is required for message create/delete ticket workflows.
GuildMembers is required for support-role checks, claim/close actions and guild member remove handling.
Guilds is required for commands, ticket channel creation/management and transcript routing.
DirectMessages is configured and used to send DM notifications; no dedicated DM message handler is currently present.
GuildVoiceStates is configured; no dedicated voice-state handler is currently present.

6. Why We Process Data
Zenial Bots process data to:
Provide configured bot features requested by server administrators
Perform moderation and safety actions, including anti-scam and anti-abuse controls
Manage tickets and support workflows
Manage temporary voice channels and voice moderation workflows
Keep operational and audit logs needed for reliability and moderation traceability

7. Legal Bases (where GDPR applies)
Art. 6(1)(b) GDPR: performance of requested bot functionality
Art. 6(1)(f) GDPR: legitimate interests in moderation, abuse prevention and platform security
Art. 6(1)(c) GDPR: compliance with legal obligations, where applicable

8. Data Storage and Retention
Primary storage is local databases.
Ticket transcripts may be generated as HTML files and stored or referenced for support workflows.
Message and moderation logs may include message text, links, attachment URLs and metadata.
Data is retained as long as needed for active bot operation, moderation traceability and support workflows.
Some records are automatically updated or removed by feature logic, but no universal auto-deletion period applies to all tables by default.

9. Data Sharing and Processors
Data may be processed through Discord platform/API/CDN infrastructure.
Data may be processed by infrastructure providers used by the operator for hosting and storage.
Data may be processed by transcript hosting endpoints used by Zenial Ticket.
Data is not sold.

10. International Transfers
Discord and related infrastructure may process data globally. Data may therefore be transferred outside your country. Appropriate contractual and technical safeguards should be used by the operator where required.

11. Security
The operator applies reasonable technical and organizational measures, including permission checks and access controls in bot workflows. No online service can guarantee absolute security.

12. User Rights
Where applicable, users may request:
Access to personal data
Rectification of inaccurate data
Erasure of data where legally possible
Restriction of processing
Objection to processing
Data portability
Complaint to a supervisory authority

Requests should be sent to the contact listed in section 2 and should include enough identifiers, for example Discord user ID and guild ID, to locate records.

13. Children
Zenial Bots are intended for Discord communities and are not specifically designed for children. Server administrators are responsible for age-appropriate server governance.

14. Policy Changes
This policy may be updated. Material changes should be announced in an appropriate Zenial information channel with an updated effective date.

15. Server Administrator Responsibilities
Server owners and administrators using Zenial Bots should:
Inform members that bot logging, moderation and ticket processing is active
Configure channels and roles responsibly
Honor valid privacy requests forwarded by users
Restrict bot access to only required channels and permissions
