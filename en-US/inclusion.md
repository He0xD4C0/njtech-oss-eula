# Repository Inclusion Rules

Updated: 2026-10-15.

Operator: {{ operator_name }}

Contact email: {{ operator_contact_email }}

## Accounts and repositories

Submissions require a valid Site account, verified email and the corresponding platform connection. Supported sources are public Git repositories on GitHub, Gitee and GitLab.com. A repository must belong directly to the connected personal account. Organization membership, collaborator access or contributions do not substitute for ownership. A platform identity can belong to only one Site account, and each Site account can retain only one connection per platform.

The default allowance is 64 retained submissions, subject to configuration. Published, pending, rejected and historical submissions count; removal releases the slot. Forks are eligible and display Fork and upstream information. Archived repositories retain inclusion and ranking eligibility and display an archive label.

## License texts and policy source

Review targets the default branch's current commit. Candidates are ordinary root files with a case-insensitive basename of LICENSE, LICENCE, COPYING, UNLICENSE or COPYRIGHT, either alone or followed by a dot, hyphen or underscore and a suffix; ordinary files immediately inside uppercase root `LICENSES/` are also read. Other subdirectories, nested files, symlinks, submodules, standalone NOTICE files and statements only in README files are not candidates.

Files must decode as UTF-8 without binary NUL. Limits are 500 candidates, 1 MiB per file and 16 MiB total. Oversized or unreadable input does not count as approval.

Classification uses complete texts from the last successfully synchronized [independent license policy repository](https://github.com/He0xD4C0/njtech-oss-license-policy), not filenames, SPDX identifiers or platform labels. The allowlist includes all licenses marked OSI-approved in a fixed SPDX release plus CC0 public-domain dedication; Unlicense is included. The denylist contains explicitly selected restrictive licenses. The repository and source manifest identify the scope. Absence from the allowlist does not automatically mean denylisting.

## Automated outcomes

- Complete allowlist coverage of all valid candidates, with other requirements met: published.
- Complete coverage by denylisted texts alone: rejected.
- No license candidates: rejected.
- Unknown, modified, incomplete or undecodable texts, added clauses or mixed allowlist/denylist texts: needs attention. The Site applies this to all candidates read, regardless of how the author describes dual licensing.

Some formatting differences and fully recognized standalone copyright holder or year notices are normalized. Substantive clauses, amounts, restrictions and uncovered symbols are retained. Template placeholders, project-specific additions or different text versions may require a policy update. A shared license name does not guarantee automatic approval.

“Needs attention” requires correcting source files or a reviewed policy update followed by automated review. Administrators have no manual approval bypass. A previously published entry that fails a new review or definitively loses eligibility becomes historical, retaining its prior public snapshot. Temporary network, platform or scanner failures alone do not establish permanent ineligibility.

## Updates and withdrawal

Submissions, policy updates, default-branch changes and platform synchronization may trigger checks. Display is not guaranteed to be real-time. You can request another review or remove a submission. When a new direct owner claims a transferred repository, the former ownership record becomes historical. A private repository or one no longer directly owned is no longer eligible as a current public entry.

Removal, disconnection or account deletion withdraws the associated entries and hides them from public historical rankings. Internal evidence, sealed statistics and backups are handled under the Privacy Policy.

## Rankings

GitHub, Gitee and GitLab.com are ranked separately, with at most ten entries per platform. Months use Asia/Shanghai. Monthly Star growth uses actual observations or the current inclusion period's publication baseline, without inventing month-start observations. Ties use ending Star count and then platform repository identifier.

Current-month rankings update with observations. Completed months are sealed and not reordered for later ineligibility; explicit withdrawal still hides entries. Historical rankings can have fewer than ten entries or gaps. Rankings do not certify code quality, academic contribution, competition eligibility or official recognition.
