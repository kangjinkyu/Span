# Privacy Policy

**Last Updated**: February 26, 2026

## The Short Version

**SPAN Finder does not collect any personal information.** No accounts. No analytics. No telemetry. No tracking. Your files are your business.

The only data ever transmitted is **anonymous crash reports** — and you can turn that off with a single toggle.

---

## What We Don't Collect

- No user accounts or sign-in required
- No file names, paths, or contents are transmitted anywhere
- No usage analytics or telemetry
- No cookies, tracking pixels, or advertising identifiers
- No data shared with or sold to third parties

## Crash Reporting (Opt-Out)

SPAN Finder includes **optional crash reporting** powered by [Sentry](https://sentry.io) to help us identify and fix bugs. This is **enabled by default** but can be turned off at any time in **Settings > Advanced > Crash Reporting**.

### What crash reports include

| Data | Purpose | Example |
|------|---------|---------|
| Exception type & stack trace | Identify the crash location in code | `NullReferenceException at ExplorerViewModel.cs:142` |
| App version | Know which release is affected | `span@1.0.1` |
| OS version | Reproduce platform-specific bugs | `Windows 11 10.0.26200` |
| .NET runtime version | Identify runtime issues | `.NET 8.0.4` |
| Memory usage | Detect out-of-memory crashes | `Working set: 280 MB` |
| View state | Understand context (no file content) | `viewMode: MillerColumns, tabCount: 3` |

### What crash reports NEVER include

- **No file names or paths** — all file paths are scrubbed before transmission (e.g., `C:\Users\***\Documents\***`)
- **No usernames or machine names** — removed before sending
- **No IP addresses or email** — `SendDefaultPii` is disabled
- **No file contents** — SPAN Finder never reads file contents for reporting
- **No browsing history or folder listings**

### How to disable

Go to **Settings > Advanced** and toggle **Crash Reporting** off. The change takes effect immediately — no restart required. When disabled, no data is transmitted and any local cache is not sent.

## Local Data Storage

SPAN Finder stores the following data **locally on your device only** to provide its functionality:

| Data | Purpose | Storage |
|------|---------|---------|
| App settings (theme, language, view options) | Preserve your preferences | Windows LocalSettings |
| Tab states (paths, view modes) | Session restore on next launch | Windows LocalSettings |
| Favorite folders | Quick access sidebar | Windows LocalSettings |
| Recent folders | Navigation convenience | Windows LocalSettings |
| FTP/SFTP credentials | Remote server reconnection | Windows ProtectedData (encrypted) |
| Crash report cache | Retry sending after network recovery | LocalAppData/Span/SentryCache |

This data **never leaves your device** except for crash reports when the feature is enabled.

## Network Communication

SPAN Finder communicates over the network **only** in these scenarios:

- **Crash reports** (if enabled): Anonymous error data sent to Sentry servers
- **FTP/SFTP connections**: Connecting to servers you explicitly configure
- **Update checks**: Querying GitHub for new versions (no user data included in the request)

No background network activity occurs outside of these actions.

## Third Parties

| Service | Purpose | Data Shared | Privacy Policy |
|---------|---------|-------------|----------------|
| Sentry (Functional Software, Inc.) | Crash reporting | Anonymous crash data only (see above) | [sentry.io/privacy](https://sentry.io/privacy/) |

No other third parties receive any data from SPAN Finder.

## Data Deletion

Uninstalling SPAN Finder removes all locally stored settings and data. You can also:

- Reset all settings within the app
- Disable crash reporting to stop all data transmission
- Delete the local crash cache at `%LocalAppData%\Span\SentryCache`

## Children's Privacy

SPAN Finder does not collect personal data from anyone, including children. Crash reports contain only technical information with no personal identifiers.

## Changes to This Policy

Any updates to this policy will be posted on this page with an updated revision date.

## Contact

For privacy-related questions, please open an issue at [GitHub Issues](https://github.com/kangjinkyu/Span/issues).
