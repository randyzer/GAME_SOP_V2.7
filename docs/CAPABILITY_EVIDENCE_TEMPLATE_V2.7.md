# Capability Evidence Record — V2.7

Status: WS-01 method candidate; no project approval or frozen release baseline is supplied by this template.

## Bound canonical identity

```json
{
  "systemVersion": "V2.7",
  "productContractVersion": "V2.7",
  "capabilityRegistryVersion": "V2.7",
  "canonicalPath": "docs/COMMERCIAL_GAME_SITE_PRODUCT_CONTRACT_V2.7.md",
  "owningArtifact": "GAME_SOP",
  "sha256": "1ff2bd01a089975c6b22bff48ca71faffe2be9c710d0123afd3ae47acc7ac24c",
  "predecessorContractVersion": "v0.2",
  "predecessorSha256": "3fe0c98d7e98f963de37fd80b3f2dbe33a822b810a1f268ec4aaef8dad90682a"
}
```

Read COMMERCIAL_GAME_SITE_PRODUCT_CONTRACT_V2.7.md Sections H/I/J/V/W/AA. This template contains evidence fields, not a second editable Registry. On contract changes rebind the hash explicitly and independently review impacted evidence.

## Record shape

Use this per capability and exact scope/build. Blank/null fields are deliberately incomplete; do not manufacture evidence to fill them.

```json
{
  "capabilityId": null,
  "canonicalContract": null,
  "sourceIdentity": null,
  "projectIdentity": null,
  "buildIdentity": null,
  "scope": "PORTABLE",
  "registryApplicability": null,
  "applicabilityDecision": {"evaluated": false, "applies": null, "selected": null, "reason": null, "decisionOwner": null, "evidenceRefs": []},
  "evidenceStatus": "NOT_RUN",
  "verifiedOutcome": null,
  "evidenceBasis": "NO_VERIFICATION_OWNER_DECISION",
  "requirementCoverage": "UNVERIFIED",
  "verificationOwner": null,
  "currentBuildReviewed": false,
  "hasKnownApplicableFailure": false,
  "evidenceRefs": [],
  "reviewer": null,
  "reviewedAt": null,
  "exception": null,
  "supersedes": [],
  "conflicts": []
}
```

`canonicalContract` equals the bound identity above. `sourceIdentity` records exact repository/root/commit/tree or a complete working-tree file-hash manifest. `buildIdentity` records the same reviewed source, mode, configuration/asset hashes, command, exit code and artifact hash; missing a build means no build-dependent result. ASSEMBLED scope requires projectIdentity. PORTABLE describes only the examined portable mechanism, not an assembled project's acceptance.

## Workflow state and outcome combinations

| evidenceStatus | verifiedOutcome | Required treatment |
| --- | --- | --- |
| NOT_RUN | null | No executed evidence; unresolved. |
| PENDING | null | Awaiting required collection/review; unresolved. |
| UNVERIFIED | null | Evidence cannot establish the obligation; unresolved. |
| OBSERVED | null | Evidence collected but no complete Verification Owner decision. |
| OBSERVED | PASS / FAIL / NOT_APPLICABLE / NOT_SELECTED / EXCEPTION | Independent full-requirement decision with exact source/build, refs, reviewer/date and owner. |

All other combinations fail. `verifiedOutcome` maps to Contract Section W's five outcomes; PENDING, BLOCK, REVISE, NOT_RUN and CONDITIONAL_PASS are not outcomes. ACTIVE/DEPRECATED/REPLACED/REMOVED belong to Registry lifecycle; neither field changes it. The Visual Evidence statuses and media lifecycle states retain their separate namespaces.

For a non-null result, evidenceBasis must be VERIFICATION_OWNER_DECISION, requirementCoverage FULL, currentBuildReviewed true, and verificationOwner must match H for the capability. Review is independent from implementation; a self-report or implementation ACCEPT cannot become capability PASS. Source/build identity and cited artifacts must be actually verified, not simply nonempty.

`registryApplicability` must exactly equal the capability's H-table category: REQUIRED / CONDITIONAL / OPTIONAL / PROHIBITED. It is distinct from the current project/build `applicabilityDecision`. Until evaluated, `evaluated=false`, `applies=null` and `selected=null`; the category itself is not a decision. Never manufacture a project decision from historical observations.

Every non-null outcome requires `evaluated=true`. REQUIRED/PROHIBITED require `applies=true`; CONDITIONAL PASS/FAIL (or approved EXCEPTION) require `applies=true`, while NOT_APPLICABLE requires `applies=false`. OPTIONAL PASS/FAIL (or approved EXCEPTION) require `selected=true`, while NOT_SELECTED requires `selected=false`. Unknown/null or contradictory decisions stop the dependent gate. REQUIRED/PROHIBITED cannot be declared inapplicable.

NOT_APPLICABLE only applies to a CONDITIONAL requirement with reason, decision owner, refs and verifier. NOT_SELECTED only applies to OPTIONAL with the same decision evidence. A known applicable failure cannot be hidden by PASS, N/A or non-selection. Approved EXCEPTION is limited to P2/NIT under Section AA, including owner, gap/impact, reason, evidence/mitigation, scope/affected routes, expiry/review date, Release Governance approval and Verification Owner acknowledgment. An expired exception becomes FAIL. No P0/P1 ordinary exception.

## Reference fixtures and real adoption

REF-A = Wiki / Commercial Editorial; REF-B = Problem Guide / Tool; REF-C = Tactical / Systems. Their original Section V fixture/media/evidence obligations all apply. PROJECT-WOG, PROJECT-BOMBFARM and PROJECT-TASK-GUIDE are separate real adoption. Many-to-many coverage notes do not substitute project PASS for deterministicReferencePass. A final release needs both groups and capability outcomes bound to the accurate candidate.

## Evidence conflicts and historical observations

Preserve earlier records and exact dates/builds; `supersedes` cites what the new review replaces, `conflicts` records unresolved contrary evidence, its owner and required re-review. New BLOCK/PENDING cannot be erased by old PASS. Build PASS cannot override human release rejection. Test totals and support labels PROVEN/PARTIAL/GAP/OUTSIDE_STARTER remain historical observations, not automatic outcomes.

A3 AX-01: OBSERVED + null; implementation accepted, browser proof pending. War of Genesis build PASS/not recommended for launch and Bomb Farm historical QA PASS/later media-rights BLOCK must remain separate accurate-version observations. No current project approval is implied.

WS01_EVIDENCE_INDEX with releaseBaseline=false is a provisional evidence index. A frozen release capability baseline is produced only after all required evidence/Reference suite/real-adoption and independent release gates; it cannot contain unresolved null outcomes as accepted results.
