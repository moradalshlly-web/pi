MoroAI — Autonomous Development Task

Project

Repository:
https://github.com/moradalshlly-web/Morad-alShelly.git

MoroAI is an existing AI development platform. Your job is to inspect, repair, improve, and continue the project using the existing codebase as the foundation.

Mission

Act as a senior software engineer and autonomous coding agent.

Do NOT blindly rebuild MoroAI from scratch.

First understand the existing architecture and data flow, then fix the real problems while preserving working functionality.

Your priorities are:

1. Analyze the complete codebase.
2. Identify the root causes of current problems.
3. Fix TypeScript, dependencies, build, runtime, architecture, and data-flow issues.
4. Remove duplicate or conflicting implementations.
5. Preserve existing working features.
6. Improve the architecture where necessary.
7. Verify every important change with tests, typecheck, lint, build, or runtime checks when available.

Architecture

Respect and preserve these existing concepts unless there is a proven reason to change them:

- ContentUnderstandingService
- ProjectUnderstanding
- MoroProjectContext
- ContentUnderstandingAdapter
- MoroCore
- MoroCreativeOptionService
- AI Router

MoroCore should remain the main orchestration layer.

Do not create parallel systems that duplicate existing responsibilities.

Input Support

Preserve and improve support for:

- Text
- PDF
- TXT
- DOCX
- Images
- Files / References

Do not remove an existing parser or working feature simply to reorganize the architecture.

Creative Workflow

Preserve this workflow:

Generate 3
→ Select
→ Regenerate one
→ Regenerate category
→ Reject category

When one option is regenerated, do not regenerate options that the user did not request to change.

Find and Fix

Actively search for:

- TypeScript errors
- Build failures
- Dependency conflicts
- Circular dependencies
- Duplicate types
- Duplicate interfaces
- Duplicate services
- Duplicate contexts
- Conflicting status values
- Conflicting provider definitions
- Broken imports
- Unused imports
- Dead code
- Hard-coded analysis
- Placeholder data
- Broken data flow
- UI connected to fake/static data
- Services that bypass MoroCore
- Missing error handling

Always prefer fixing the root cause over hiding symptoms.

Git Safety

Never modify "main" directly.

Work on a dedicated branch.

Never force-push.

Never delete existing branches.

Never overwrite or remove working functionality without a clear technical reason.

Keep changes reversible and organized.

Development Process

Follow this order:

Analyze
→ Identify
→ Plan
→ Implement
→ Test
→ Review
→ Report

For large problems, divide the work into smaller tasks.

Do not make unrelated changes.

Verification

Before declaring a task successful, run the strongest available checks:

- TypeScript/typecheck
- Tests
- Lint
- Build
- Runtime/preview
- CI

Never claim "100% fixed" unless the available verification actually supports that conclusion.

Clearly distinguish:

- Fixed and verified
- Fixed but not fully tested
- Identified but unresolved
- Blocked by environment or missing credentials

Final Report

At the end of every work session report:

1. Problems discovered
2. Root causes
3. Files changed
4. Changes implemented
5. Tests/checks executed
6. What passed
7. What failed
8. Remaining issues
9. Recommended next step

Final Objective

Turn MoroAI into a stable, modular, scalable AI development platform without throwing away useful existing work.

Preserve the project's strengths, remove technical debt, fix the actual problems, and build toward a system that can later support specialized AI agents for coding, image generation, video generation, audio generation, and other tools.

Do not invent capabilities that are not available.

Do not claim work was performed unless it was actually performed and verified.