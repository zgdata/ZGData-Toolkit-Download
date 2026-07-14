# ZgData Toolkit - Changelog

## 1.1.0 - 2026-07-14

### Phase 1 - Multi-cloud configuration foundation
- Added a `CloudTargets` configuration list while preserving legacy iPerf settings for compatibility.
- Added Alwyzon, Hetzner and a disabled DataBox target.
- Added `SingleTarget` and `CompareTargets` test-mode models.

### Phase 2 - Single-target UI and execution
- Added Single target and Compare cloud targets controls.
- Added selectable cloud targets.
- Connected Single target mode to ping, iPerf, DNS, traceroute and Internet Quality.
- Kept SQL as a separate optional endpoint.

### Phase 3 - Compare engine and report
- Added concurrent continuous ping monitoring for selected targets.
- Added strictly sequential iPerf upload/download execution.
- Added rotating iPerf runs for Extended and Burn-In profiles.
- Added per-target DNS and traceroute results.
- Added Cloud Target Comparison and Best measured network path.
- Added detailed per-target report sections.

### Phase 4 - Reliability and report wording
- Added parallel warm-up pings before measured monitoring.
- Excluded warm-up samples from packet loss, availability, charts and incidents.
- Kept real timeouts during measured monitoring fully recorded.
- Clarified that Quick does not run traceroute.
- Renamed Location to Provider / region in comparison tables.

### Phase 5 - UI, unified report and client ISP
- Moved progress percentage and status inside the progress bar for smaller screens.
- Fixed clipped Compare cloud targets text.
- Added an in-app results table showing all selected providers.
- Added side-by-side comparison tables for Internet Quality, ping, iPerf, DNS and traceroute.
- Collapsed detailed target charts for easier report navigation.
- Added client internet provider, public IP, ASN and approximate public-IP location.

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
