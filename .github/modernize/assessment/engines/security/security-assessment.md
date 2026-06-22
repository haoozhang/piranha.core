# Security Assessment Report

**Generated:** 06/22/2026 10:30:17

## Summary

| Metric | Count |
|--------|-------|
| Total Findings | 12 |
| CVE Vulnerabilities | 8 |
| CWE Vulnerabilities | 4 |
| Total Rules Assessed | 59 |
| Rules Passed | 55 |

### By Severity

| Severity | Count |
|----------|-------|
| mandatory | 9 |
| optional | 1 |
| potential | 2 |

## CVE Findings (Dependency Vulnerabilities)
### CVE-2026-32933: AutoMapper Vulnerable to Denial of Service (DoS) via Uncontrolled Recursion
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** data/Piranha.Data.EF/Piranha.Data.EF.csproj:19

[CVE-2026-32933](https://github.com/advisories/GHSA-rvv3-g6hj-g44x): AutoMapper Vulnerable to Denial of Service (DoS) via Uncontrolled Recursion

Severity: HIGH

Affected dependencies:
  - AutoMapper:12.0.1 (top-level, declared at data/Piranha.Data.EF/Piranha.Data.EF.csproj:19)

Vulnerable version range: < 15.1.1

Recommended fix:
  - Upgrade AutoMapper to 15.1.1 or later
### CVE-2023-36414: Azure Identity SDK Remote Code Execution Vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** data/Piranha.Data.EF.SQLServer/Piranha.Data.EF.SQLServer.csproj, identity/Piranha.AspNetCore.Identity.SQLServer/Piranha.AspNetCore.Identity.SQLServer.csproj, examples/RazorWeb/RazorWeb.csproj

[CVE-2023-36414](https://github.com/advisories/GHSA-5mfx-4wcx-rv27): Azure Identity SDK Remote Code Execution Vulnerability

Severity: HIGH

Affected dependencies:
  - Azure.Identity:1.7.0 (transitive, in Piranha.Data.EF.SQLServer, Piranha.AspNetCore.Identity.SQLServer, RazorWeb)

Vulnerable version range: < 1.10.2

Recommended fix:
  - Upgrade Azure.Identity to 1.10.2 or later (already at 1.11.4 in some projects — consolidate to that version)
### CVE-2024-0056: Microsoft.Data.SqlClient and System.Data.SqlClient vulnerable to SQL Data Provider Security Feature Bypass
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** data/Piranha.Data.EF.SQLServer/Piranha.Data.EF.SQLServer.csproj, identity/Piranha.AspNetCore.Identity.SQLServer/Piranha.AspNetCore.Identity.SQLServer.csproj, examples/RazorWeb/RazorWeb.csproj

[CVE-2024-0056](https://github.com/advisories/GHSA-98g6-xh36-x2p7): Microsoft.Data.SqlClient and System.Data.SqlClient vulnerable to SQL Data Provider Security Feature Bypass

Severity: HIGH

Affected dependencies:
  - Microsoft.Data.SqlClient:5.1.1 (transitive, in Piranha.Data.EF.SQLServer, Piranha.AspNetCore.Identity.SQLServer, RazorWeb)

Vulnerable version range: >= 5.0.0, < 5.1.3

Recommended fix:
  - Upgrade Microsoft.Data.SqlClient to 5.1.3 or later (already at 5.1.6 in some projects — consolidate to that version)
### CVE-2024-43483: Microsoft Security Advisory CVE-2024-43483 | .NET Denial of Service Vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** data/Piranha.Data.EF.SQLite/Piranha.Data.EF.SQLite.csproj, data/Piranha.Data.EF.SQLServer/Piranha.Data.EF.SQLServer.csproj, data/Piranha.Data.EF/Piranha.Data.EF.csproj, examples/MvcWeb/MvcWeb.csproj

[CVE-2024-43483](https://github.com/advisories/GHSA-qj66-m88j-hmgj): Microsoft Security Advisory CVE-2024-43483 | .NET Denial of Service Vulnerability

Severity: HIGH

Affected dependencies:
  - Microsoft.Extensions.Caching.Memory:8.0.0 (transitive, in multiple projects)

Vulnerable version range: >= 8.0.0-preview.1.23110.8, <= 8.0.0

Recommended fix:
  - Upgrade Microsoft.Extensions.Caching.Memory to 8.0.1 or later
### CVE-2025-6965: SQLitePCLRaw.lib.e_sqlite3 has a vulnerable dependency on SQLite
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** data/Piranha.Data.EF.SQLite/Piranha.Data.EF.SQLite.csproj, identity/Piranha.AspNetCore.Identity.SQLite/Piranha.AspNetCore.Identity.SQLite.csproj, examples/MvcWeb/MvcWeb.csproj, examples/RazorWeb/RazorWeb.csproj, test/Piranha.Tests/Piranha.Tests.csproj

[CVE-2025-6965](https://github.com/advisories/GHSA-2m69-gcr7-jv3q): SQLitePCLRaw.lib.e_sqlite3 has a vulnerable dependency on SQLite

Severity: HIGH

Affected dependencies:
  - SQLitePCLRaw.lib.e_sqlite3:2.1.6 (transitive)
  - SQLitePCLRaw.lib.e_sqlite3:2.1.10 (transitive)

Vulnerable version range: <= 2.1.11

Recommended fix:
  - Upgrade SQLitePCLRaw.lib.e_sqlite3 to a version > 2.1.11 when available, or monitor for a patched release
### CVE-2024-38095: Microsoft Security Advisory CVE-2024-38095 | .NET Denial of Service Vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** data/Piranha.Data.EF.SQLServer/Piranha.Data.EF.SQLServer.csproj, identity/Piranha.AspNetCore.Identity.SQLServer/Piranha.AspNetCore.Identity.SQLServer.csproj, examples/RazorWeb/RazorWeb.csproj

[CVE-2024-38095](https://github.com/advisories/GHSA-447r-wph3-92pm): Microsoft Security Advisory CVE-2024-38095 | .NET Denial of Service Vulnerability

Severity: HIGH

Affected dependencies:
  - System.Formats.Asn1:5.0.0 (transitive, in Piranha.Data.EF.SQLServer, Piranha.AspNetCore.Identity.SQLServer, RazorWeb)

Vulnerable version range: >= 5.0.0-preview.7.20364.11, < 6.0.1

Recommended fix:
  - Upgrade System.Formats.Asn1 to 6.0.1 or later
### CVE-2024-43485: Microsoft Security Advisory CVE-2024-43485 | .NET Denial of Service Vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** core/Piranha.AspNetCore/Piranha.AspNetCore.csproj, data/Piranha.Data.EF.SQLite/Piranha.Data.EF.SQLite.csproj, data/Piranha.Data.EF/Piranha.Data.EF.csproj, examples/MvcWeb/MvcWeb.csproj, examples/RazorWeb/RazorWeb.csproj

[CVE-2024-43485](https://github.com/advisories/GHSA-8g4q-xg66-9fp4): Microsoft Security Advisory CVE-2024-43485 | .NET Denial of Service Vulnerability

Severity: HIGH

Affected dependencies:
  - System.Text.Json:8.0.0 (transitive, in multiple projects)

Vulnerable version range: >= 8.0.0, <= 8.0.4

Recommended fix:
  - Upgrade System.Text.Json to 8.0.5 or later
### CVE-2024-30105: Microsoft Security Advisory CVE-2024-30105 | .NET Denial of Service Vulnerability
- **Severity:** mandatory
- **Story Points:** 1
- **Files:** core/Piranha.AspNetCore/Piranha.AspNetCore.csproj, data/Piranha.Data.EF.SQLite/Piranha.Data.EF.SQLite.csproj, data/Piranha.Data.EF/Piranha.Data.EF.csproj, examples/MvcWeb/MvcWeb.csproj, examples/RazorWeb/RazorWeb.csproj

[CVE-2024-30105](https://github.com/advisories/GHSA-hh2w-p6rv-4g7w): Microsoft Security Advisory CVE-2024-30105 | .NET Denial of Service Vulnerability

Severity: HIGH

Affected dependencies:
  - System.Text.Json:8.0.0 (transitive, in multiple projects)

Vulnerable version range: >= 7.0.0, < 8.0.4

Recommended fix:
  - Upgrade System.Text.Json to 8.0.4 or later
## CWE Findings (Code-Level Vulnerabilities)
### CWE-567: Unsynchronized Access to Shared Data in a Multithreaded Context
- **Category:** Concurrency & Synchronization
- **Severity:** potential
- **Story Points:** 5
- **Files:** core/Piranha/Extend/Fields/SelectField.cs

In SelectField.cs, the static field 'IsInitialized' (line 34) is declared as a plain bool without the 'volatile' keyword. The InitMetaData() method (lines 174-196) uses double-checked locking: the outer check at line 176 reads 'IsInitialized' without any synchronization, before acquiring the Mutex lock at line 179. Without 'volatile', the .NET memory model does not guarantee that writes to 'IsInitialized' made by one thread are immediately visible to other threads reading outside the lock, potentially allowing multiple threads to pass the outer check and enter the lock simultaneously or observe a stale value. The static '_items' list (line 24) is also written by multiple threads without consistent synchronization at the read path.
### CWE-778: Insufficient Logging
- **Category:** Credentials & Secrets
- **Severity:** potential
- **Story Points:** 3
- **Files:** core/Piranha.Manager.LocalAuth/Areas/Manager/Pages/Login.cshtml.cs, core/Piranha.WebApi/PostApiController.cs, core/Piranha.WebApi/PageApiController.cs

Failed authentication and authorization events are not logged. In Login.cshtml.cs (line 98-102), when login fails (SignIn returns non-Succeeded result), the event is silently discarded — only a UI error message is added, no security log entry is written. Similarly, in the API controllers (e.g., PostApiController.cs, PageApiController.cs), when authorization checks fail and Unauthorized() is returned, there is no log entry recording the unauthorized access attempt, the requesting user, or the requested resource. This makes it difficult to detect brute-force attacks or unauthorized access patterns.
### CWE-22: Improper Limitation of a Pathname to a Restricted Directory ('Path Traversal')
- **Category:** File & Path Security
- **Severity:** optional
- **Story Points:** 8
- **Files:** core/Piranha.Local.FileStorage/FileStorageSession.cs

In FileStorageSession.cs, file paths are constructed by string concatenation: '_basePath + path' (lines 48, 50, 73, 94, 112, 114) where 'path' comes from GetResourceName() which builds '{media.Id}/{filename}'. The filename originates from user-supplied upload data. While the Manager service layer applies Path.GetFileName() (Piranha.Manager/Services/MediaService.cs:252) for the upload controller path, the core storage layer (Piranha/Services/Internal/MediaService.cs:247) only replaces spaces, performing no path traversal validation. If the core API is accessed directly, a filename containing '../' sequences under UniqueFolderNames naming could escape the '_basePath' directory boundary.
### CWE-502: Deserialization of Untrusted Data
- **Category:** Injection Attacks
- **Severity:** mandatory
- **Story Points:** 13
- **Files:** core/Piranha/Cache/Internal/DistributedCache.cs

In DistributedCache.cs (lines 29-32, 42), the Newtonsoft.Json serializer is configured with TypeNameHandling = TypeNameHandling.All. When deserializing data from the distributed cache (e.g., Redis) at line 42 via JsonConvert.DeserializeObject<T>(json, _jsonSettings), the '\' property embedded in the cached JSON can cause Newtonsoft.Json to instantiate arbitrary .NET types. If an attacker is able to poison the cache backend, they could inject malicious '\' references leading to Remote Code Execution (RCE). This is a well-known gadget chain attack vector in Newtonsoft.Json with TypeNameHandling.All.

