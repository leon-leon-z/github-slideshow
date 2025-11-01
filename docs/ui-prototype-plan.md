# Live Street View – UI Prototype & User Testing Plan

## Objectives
- Validate the map-first request discovery experience.
- Assess the clarity of the request submission and response locking workflow.
- Measure perceived value of reward points and overall trust in the platform.

## Prototype Scope
1. **Navigation shell** reflecting the bottom tab bar (*Requests*, *Add Request*, *My Requests*).
2. **Map view** with clustered request markers and a detail sheet showing countdown, reward, and respond CTA.
3. **Add Request flow** including Google Places autocomplete stub, optional comments, and reward estimate input.
4. **My Requests dashboard** with state filters (Open, Awaiting Review, Completed, Rejected) and sample response cards.
5. **Profile drawer** showing reward balance, basic profile info, and settings entry points.

Prototype fidelity: start with high-fidelity Figma mockups linked with interactive hotspots; evolve to a clickable web prototype (React + Mapbox GL JS or Google Maps JS SDK) backed by mocked JSON data.

## Tooling
- **Design:** Figma for component library, responsive layout variants, and interactive prototype flows.
- **Prototyping:**
  - Phase 1: Figma prototype with overlays, smart animations, and flow branching.
  - Phase 2: React (Next.js) or Expo Web PWA that consumes local JSON fixtures for requests, responses, and user profile.
- **Collaboration:** Figma comments, Loom walkthroughs, and Notion/Confluence for documentation.
- **Version control:** GitHub for the clickable prototype code with feature branches mapped to UI tickets.

## Implementation Milestones
| Week | Deliverable | Details |
|------|-------------|---------|
| 1 | UX audit & component inventory | Confirm navigation hierarchy, identify missing states, document accessibility considerations. |
| 2 | Figma high-fidelity prototype | Link all primary flows; include edge cases (locked request, rejected response). |
| 3 | Clickable web prototype (MVP) | Implement map view, request detail sheet, add-request form with Places autocomplete stub, and My Requests list using mock data. |
| 4 | Prototype refinements | Add basic analytics hooks (console logging), loading/error states, and responsive tweaks for tablet/mobile. |

## User Testing Plan
1. **Recruitment**
   - Target 8–10 participants split between travelers and local gig seekers.
   - Screen for smartphone usage, familiarity with map apps, and willingness to share location-based media.
2. **Test Format**
   - Conduct 45-minute moderated remote sessions via Zoom.
   - Provide participants with prototype link (Figma for early tests, web PWA for later sessions).
   - Use think-aloud protocol while completing scripted tasks.
3. **Core Tasks**
   1. Discover and open a nearby request from the map.
   2. Submit a new request for a specified landmark, including optional comment.
   3. Review a response, accept it, and award points.
   4. Reject a response with feedback and verify that the request reopens.
   5. Check reward balance and profile info.
4. **Metrics & Observations**
   - Task completion rate & time on task.
   - SUS (System Usability Scale) score per participant.
   - Qualitative feedback: trust cues, clarity of the five-minute SLA, perceived fairness of reward system.
   - Record friction points (e.g., autocomplete expectations, confusion over locked states).
5. **Post-Session Synthesis**
   - Affinity map observations in FigJam.
   - Prioritize issues by severity and effort; feed into backlog for prototype updates.
   - Summarize findings and recommendations in a shareable report.

## Success Criteria
- ≥80% task completion without moderator intervention.
- SUS score ≥75.
- Participants report clear understanding of request lifecycle and reward mechanics.
- Identified design issues have actionable next steps for MVP build.

## Next Steps After Testing
- Iterate on prototype to address high-severity issues.
- Validate technical feasibility for native implementations (camera capture, push notifications).
- Align with product and engineering on MVP scope, timelines, and KPIs based on testing insights.
