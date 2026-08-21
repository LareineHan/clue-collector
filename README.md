# Clue Collector v0.2

Defensive phishing URL correlation tool.

Key fixes:
- arbitrary pasted text is accepted, but only http/https URLs are parsed;
- repeated clues are current-batch only and appear first;
- saved history is opt-in and isolated on its own tab;
- Clear history clears only saved history;
- CNAME enrichment recognizes custom tracking domains for Mandrill, SendGrid, Mailgun, and some HubSpot hosts;
- SharePoint tenant and OneDrive personal namespaces are extracted;
- Google Drive/Docs resource IDs are resource pivots, never account IDs;
- DocuSign shared server designations are suppressed; repeated opaque DocuSign values are campaign/resource clues only;
- shared provider domains are never treated as sender linkage;
- KQL pivot drafts are produced only from supported repeated clues.

Push to a GitHub repo connected to Cloudflare Workers/Pages.
