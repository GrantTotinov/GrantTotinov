## Support my work

I build .NET libraries, ASP.NET Core security tooling and browser extensions, and I contribute to the .NET ecosystem.
I'm a member of the **.NET Foundation** and I spend most of my time on open source, mainly around .NET and ASP.NET Core.
If my work helps you, you can sponsor me on GitHub or buy me a coffee. I'm also saving for a PhD, so even a small amount goes a long way.

<p>
  <a href="https://github.com/sponsors/GrantTotinov"><img src="https://img.shields.io/badge/GitHub%20Sponsors-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white" alt="GitHub Sponsors" /></a>
  <a href="https://buymeacoffee.com/granttotinov"><img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black" alt="Buy Me a Coffee" /></a>
</p>

<p>
  <a href="https://dotnetfoundation.org/"><img src="https://img.shields.io/badge/Member-.NET%20Foundation-512BD4?style=for-the-badge&labelColor=2B2B2B" alt=".NET Foundation Member" /></a>
  <a href="https://learn.microsoft.com/en-us/answers/"><img src="https://img.shields.io/badge/Microsoft-Q%26A%20Champion-0078D4?style=for-the-badge&labelColor=2B2B2B" alt="Microsoft Q&amp;A Champion" /></a>
</p>

## Projects

- **[PixelForge](https://github.com/GrantTotinov/PixelForge)**: MIT image processing for .NET, built on SkiaSharp. Familiar Load / Mutate / Resize / Save API, no license key and safe defaults for user uploads. On [NuGet](https://www.nuget.org/packages/PixelForge).
- **[UploadGuard](https://github.com/GrantTotinov/UploadGuard)**: secure file uploads for ASP.NET Core. Magic-byte detection, allow-list policies, zip bomb, Office macro, PDF JavaScript and SVG script checks, ClamAV scanning and image re-encoding. On [NuGet](https://www.nuget.org/packages/UploadGuard).
- **[AI Exporter](https://github.com/GrantTotinov/AIExporter)**: a free browser extension that exports ChatGPT, Claude, Gemini, DeepSeek, Grok, Perplexity, Copilot and other AI chats to PDF, Word, HTML, Markdown, JSON, CSV or Excel, images included. Available for [Chrome](https://chromewebstore.google.com/detail/gptchatdownloader/objkcakdcilfaphifjfcgfamlnnbinjc), [Firefox](https://addons.mozilla.org/en-US/firefox/addon/aiexporter/) and [Edge](https://microsoftedge.microsoft.com/addons/detail/ai-exporter-chatgpt-cla/ogkpijnjfiebjpcllkkgablmiijgjhim), with its own [website](https://granttotinov.github.io/AIExporter/).
- **[aspnetcore-security-bench](https://github.com/GrantTotinov/aspnetcore-security-bench)**: vulnerable and fixed ASP.NET Core app pairs for silent security misconfigurations, verified on .NET 8 and 10, with an evaluation of which tools detect them.
- Also: [AiChatRagSystem](https://github.com/GrantTotinov/AiChatRagSystem), Q&A over your own documents with RAG (.NET 8, React, Ollama), [GrantFoodsMAUI](https://github.com/GrantTotinov/GrantFoodsMAUI), a cross-platform food ordering app in .NET MAUI, and [uni-event-app](https://github.com/GrantTotinov/uni-event-app), a university events app in React Native.

## Open source contributions

- **Microsoft / .NET**: [ASP.NET Core](https://github.com/dotnet/aspnetcore/pulls?q=is%3Apr+author%3AGrantTotinov) and the [ASP.NET Core documentation](https://github.com/dotnet/AspNetCore.Docs/pulls?q=is%3Apr+author%3AGrantTotinov+is%3Amerged). Most of my work is on security in authentication, Identity and passkeys.
  - **Passkeys (WebAuthn)**: [validation of the COSE algorithm and curve](https://github.com/dotnet/aspnetcore/pull/68834) when decoding a passkey public key, and [a controlled sign-in failure instead of an unhandled exception](https://github.com/dotnet/aspnetcore/pull/67539) when the passkey session challenge has expired.
  - **Authorization**: the routing guard for unprocessed authorization metadata [now also covers `AuthorizationPolicy` and `IAuthorizationRequirementData`](https://github.com/dotnet/aspnetcore/pull/67742), so a misconfigured pipeline fails fast instead of silently skipping authorization.
  - **Identity**: the default confirmation and password-reset emails [now tell recipients who didn't start the action that they can ignore them](https://github.com/dotnet/aspnetcore/pull/66747).
  - **Documentation**: antiforgery HTTP method limitations and the `HttpMethodOverride` interaction, in the [API docs](https://github.com/dotnet/aspnetcore/pull/66772) and on [Microsoft Learn](https://github.com/dotnet/AspNetCore.Docs/pull/37224), and [rate limiter ordering with `UseStatusCodePagesWithReExecute`](https://github.com/dotnet/AspNetCore.Docs/pull/37964).
  - **In review**: [two-factor authentication for external-login sign-in](https://github.com/dotnet/aspnetcore/pull/69075) in the Identity UI, [TLS channel binding for forwarded client certificates](https://github.com/dotnet/aspnetcore/pull/69982), [no cookie renewal after failed principal validation](https://github.com/dotnet/aspnetcore/pull/70028), [a depth limit for nested LDAP groups in Negotiate](https://github.com/dotnet/aspnetcore/pull/70041), [failed updates surfaced from the Identity API `/manage/2fa` endpoint](https://github.com/dotnet/aspnetcore/pull/69966) and [`MapStaticAssets` conventions on the fallback endpoint](https://github.com/dotnet/aspnetcore/pull/69960).
  - **Bug reports**: [Identity pages returning 500 for a malformed reset or confirmation code](https://github.com/dotnet/aspnetcore/issues/70070), and [`RedisOutputCacheStore` releasing the wrong connection on forced reconnect](https://github.com/dotnet/aspnetcore/issues/70029).
- **Spectre.Console**: [escaping of interpolated arguments in markup](https://github.com/spectreconsole/spectre.console/pull/2118) and [`Align` measuring with an explicit width](https://github.com/spectreconsole/spectre.console/pull/2101).
- **Tiptap**: [`getReferencedVirtualElement` forwarded to the plugin](https://github.com/ueberdosis/tiptap/pull/7832) in the React drag handle.
- **Microsoft Q&A**: I answer .NET and ASP.NET Core questions as a [Q&A Champion](https://learn.microsoft.com/en-us/answers/).

## Tech stack

<img src="https://skillicons.dev/icons?i=cs,dotnet,py,ts,react,postgres,docker,azure,aws" alt="C#, .NET, Python, TypeScript, React, PostgreSQL, Docker, Azure, AWS" />

Also ASP.NET Core, .NET MAUI, React Native, SQL Server, REST and OpenAPI, LLMs and RAG.

---

[Website](https://granttotinov.github.io/) · [NuGet](https://www.nuget.org/profiles/GrantTotinov) · [GitHub Sponsors](https://github.com/sponsors/GrantTotinov)
