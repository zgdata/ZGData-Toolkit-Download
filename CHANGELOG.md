# ZgData Toolkit - Changelog

## 1.2.0 - 2026-07-15

### Apross Client Monitor
- Added local Apross.exe process discovery and selection by PID, Windows user and window title.
- Added child-process and WebView2 tracking.
- Added process health sampling for CPU, memory, private memory, handles, GDI, USER objects and responding state.
- Added TCP endpoint tracking and classification for SQL, Web/API, file-share, file-transfer, mail and other connections.
- Added local/LAN versus public/cloud backend classification.
- Added operator problem markers and unified process/network incident timeline.
- Added HTML and CSV exports for process samples, connections and timeline events.
- Added optional circular Windows ETL packet trace for administrator sessions.

### SQL live correlation
- Added a separate SQL monitoring connection for reading server-side diagnostic data.
- Added correlation between the local Apross TCP port and SQL Server sessions.
- Added SPID, login, program, database, command, elapsed time, waits, blocking, CPU, reads, writes and optional SQL text.
- Added SQL access test and server-state permission validation.
- Added SQL Server helper scripts for checking, granting and revoking monitoring permissions.
- Clarified the distinction between Windows user, Apross application user and SQL monitoring login.
- SQL passwords are not persisted to reports, CSV, settings.json or source files.

### Reliability and fixes
- Fixed PowerShell SQL connection-string keyword handling.
- Fixed a C# null-coalescing build error in the SQL correlation service.
- Fixed duplicate SQL query variables.
- Fixed startup handling when the temporary local-port file is empty.
- Removed nullable-return warnings in the internet-provider lookup service.

## 1.1.0 - 2026-07-14

### Multi-cloud configuration and user interface
- Added `Single target` and `Compare cloud targets` modes.
- Added active Alwyzon and Hetzner targets and a disabled DataBox target prepared for later activation.
- Added estimated duration for compare runs.
- Kept SQL testing as a separate optional endpoint.

### Multi-cloud diagnostics engine
- Added concurrent continuous ping monitoring for all selected targets.
- Added strictly sequential iPerf3 upload/download execution.
- Added rotating periodic iPerf runs for Extended and Burn-In profiles.
- Added per-target DNS and traceroute results.
- Added parallel warm-up pings that are excluded from measured statistics and incidents.

### Results and reports
- Added an in-app comparison table showing every selected target.
- Added `Best measured network path` without presenting it as an overall provider ranking.
- Added side-by-side report tables for Internet Quality, ping, iPerf3, DNS and traceroute.
- Kept detailed per-target charts available in collapsible sections.
- Added client internet provider/organization, public IP, ASN and approximate public-IP location.

### UI and reliability fixes
- Moved progress percentage and status inside the progress bar for smaller screens.
- Fixed clipped `Compare cloud targets` text.
- Clarified that Quick does not run traceroute.
- Preserved real packet loss and timeout incidents after warm-up.

### Infrastructure
- Added reusable Linux install and verification scripts for diagnostics nodes.
- Deployed and verified the Hetzner Falkenstein node on TCP 5201.
- Preserved the existing SVN service on TCP 3690.
- Prepared the DataBox node configuration for later activation.

## 1.0.0 - 2026-07-13
- Initial Windows WPF .NET 8 release.
- Quick, Standard, Extended and Burn-In profiles.
- Internet Quality, continuous ping, optional SQL TCP monitoring, iPerf3, DNS and traceroute.
- STOP with partial HTML report.
- Computer/network information, incident timeline and inline SVG charts.
- Self-contained Windows x64 publish package.
