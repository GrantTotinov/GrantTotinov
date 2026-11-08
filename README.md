## Thanks for stopping by!

I'm a member of the **.NET Foundation** and I spend most of my time on open source, building .NET libraries, ASP.NET Core security tooling and browser extensions, and contributing to ASP.NET Core and the wider .NET ecosystem.
Everything I make is free to use. If something here saved you some time, you can say thanks by sponsoring me on GitHub or buying me a coffee. I'm also saving up for a PhD, so every little bit really helps.

<p>
  <a href="https://github.com/sponsors/GrantTotinov"><img src="https://img.shields.io/badge/GitHub%20Sponsors-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white" alt="GitHub Sponsors" /></a>
  <a href="https://buymeacoffee.com/granttotinov"><img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black" alt="Buy Me a Coffee" /></a>
</p>

<p>
  <a href="https://dotnetfoundation.org/"><img src="https://img.shields.io/badge/Member-.NET%20Foundation-512BD4?style=for-the-badge&labelColor=2B2B2B" alt=".NET Foundation Member" /></a>
  <a href="https://learn.microsoft.com/en-us/answers/"><img src="https://img.shields.io/badge/Microsoft-Q%26A%20Champion-0078D4?style=for-the-badge&labelColor=2B2B2B" alt="Microsoft Q&amp;A Champion" /></a>
</p>

## Free tools I build

- **[AI Exporter](https://github.com/GrantTotinov/AIExporter)**: saves your ChatGPT, Claude, Gemini and other AI chats as PDF, Word, Markdown and more. 400+ users, rated 5/5. [Chrome](https://chromewebstore.google.com/detail/gptchatdownloader/objkcakdcilfaphifjfcgfamlnnbinjc) · [Firefox](https://addons.mozilla.org/en-US/firefox/addon/aiexporter/) · [Edge](https://microsoftedge.microsoft.com/addons/detail/ai-exporter-chatgpt-cla/ogkpijnjfiebjpcllkkgablmiijgjhim)
- **[PixelForge](https://github.com/GrantTotinov/PixelForge)**: MIT image processing for .NET with an ImageSharp-style API, no license key and safe defaults for user uploads. [NuGet](https://www.nuget.org/packages/PixelForge)
- **[UploadGuard](https://github.com/GrantTotinov/UploadGuard)**: secure file uploads for ASP.NET Core that catch zip bombs, macros, PDF JavaScript and disguised files. [NuGet](https://www.nuget.org/packages/UploadGuard)
- **[aspnetcore-security-bench](https://github.com/GrantTotinov/aspnetcore-security-bench)**: a benchmark and [technical report](https://doi.org/10.5281/zenodo.23822216) on ASP.NET Core misconfigurations that CodeQL, Semgrep and the .NET analyzers all miss.
- Earlier projects: [AiChatRagSystem](https://github.com/GrantTotinov/AiChatRagSystem), [GrantFoodsMAUI](https://github.com/GrantTotinov/GrantFoodsMAUI) and [uni-event-app](https://github.com/GrantTotinov/uni-event-app).

## Open source contributions

- **[ASP.NET Core](https://github.com/dotnet/aspnetcore/pulls?q=is%3Apr+author%3AGrantTotinov)**: security work across authentication, Identity and passkeys.
  - **Passkeys (WebAuthn)**: [COSE algorithm and curve validation](https://github.com/dotnet/aspnetcore/pull/68834) when decoding a passkey public key, and [a controlled sign-in failure instead of an unhandled exception](https://github.com/dotnet/aspnetcore/pull/67539) when the passkey challenge has expired.
  - **Identity and two-factor authentication**: [two-factor authentication on external-login sign-in](https://github.com/dotnet/aspnetcore/pull/69075) in the Identity UI, [failed `/manage/2fa` updates surfaced](https://github.com/dotnet/aspnetcore/pull/69966) in the Identity API, [clearer default emails](https://github.com/dotnet/aspnetcore/pull/66747) for people who didn't ask for them, and [a 500 error on malformed reset and confirmation codes](https://github.com/dotnet/aspnetcore/issues/70070).
  - **Authentication**: [TLS channel binding kept](https://github.com/dotnet/aspnetcore/pull/69982) when client certificates are forwarded, [no cookie renewal after failed principal validation](https://github.com/dotnet/aspnetcore/pull/70028), and [a depth limit for nested LDAP groups](https://github.com/dotnet/aspnetcore/pull/70041) in Negotiate.
  - **Authorization**: the routing guard for unprocessed authorization metadata, [extended to `AuthorizationPolicy` and `IAuthorizationRequirementData`](https://github.com/dotnet/aspnetcore/pull/67742) so a misconfigured pipeline fails fast instead of silently skipping authorization.
  - **Antiforgery and rate limiting**: antiforgery HTTP method limitations documented in the [API reference](https://github.com/dotnet/aspnetcore/pull/66772) and on [Microsoft Learn](https://github.com/dotnet/AspNetCore.Docs/pull/37224), and [rate limiter ordering](https://github.com/dotnet/AspNetCore.Docs/pull/37964). These are the findings behind the technical report above.
  - **Middleware and caching**: [`MapStaticAssets` conventions on the fallback endpoint](https://github.com/dotnet/aspnetcore/pull/69960) and [`RedisOutputCacheStore` releasing the wrong connection on reconnect](https://github.com/dotnet/aspnetcore/issues/70029).
- **[Spectre.Console](https://github.com/spectreconsole/spectre.console/pulls?q=is%3Apr+author%3AGrantTotinov+is%3Amerged)**: [escaping of interpolated arguments in markup](https://github.com/spectreconsole/spectre.console/pull/2118) and [`Align` measuring with an explicit width](https://github.com/spectreconsole/spectre.console/pull/2101).
- **[Tiptap](https://github.com/ueberdosis/tiptap/pulls?q=is%3Apr+author%3AGrantTotinov+is%3Amerged)**: [`getReferencedVirtualElement` forwarded to the plugin](https://github.com/ueberdosis/tiptap/pull/7832) in the React drag handle.
- **Microsoft Q&A**: I answer .NET and ASP.NET Core questions as a [Q&A Champion](https://learn.microsoft.com/en-us/answers/).

## Tech stack

<img src="https://skillicons.dev/icons?i=cs,dotnet,py,ts,react,postgres,docker,azure,aws" alt="C#, .NET, Python, TypeScript, React, PostgreSQL, Docker, Azure, AWS" />

Also ASP.NET Core, .NET MAUI, React Native, SQL Server, REST and OpenAPI, LLMs and RAG.

---

[Website](https://granttotinov.github.io/) · [NuGet](https://www.nuget.org/profiles/GrantTotinov) · [ORCID](https://orcid.org/0009-0002-8014-409X) · [GitHub Sponsors](https://github.com/sponsors/GrantTotinov)
