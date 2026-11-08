## Support my work

I'm a member of the **.NET Foundation** and I spend most of my time on open source, building .NET libraries, ASP.NET Core security tooling and browser extensions, and contributing to ASP.NET Core and the wider .NET ecosystem.
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

- **[AI Exporter](https://github.com/GrantTotinov/AIExporter)**: a free browser extension with 400+ users and a 5/5 rating on the Chrome Web Store and Firefox Add-ons. It exports conversations from 15 AI chat sites, including ChatGPT, Claude, Gemini, DeepSeek, Grok, Perplexity and Copilot, to 9 formats such as PDF, Word, Excel and Markdown, images included. Instead of scraping the page, it reads each site's own conversation API, so long chats and branches come out complete. Everything runs locally in the browser, with automatic backups to a folder or a private GitHub repository and an interface in 13 languages. Get it for [Chrome](https://chromewebstore.google.com/detail/gptchatdownloader/objkcakdcilfaphifjfcgfamlnnbinjc), [Firefox](https://addons.mozilla.org/en-US/firefox/addon/aiexporter/) or [Edge](https://microsoftedge.microsoft.com/addons/detail/ai-exporter-chatgpt-cla/ogkpijnjfiebjpcllkkgablmiijgjhim), or visit the [website](https://granttotinov.github.io/AIExporter/).
- **[PixelForge](https://github.com/GrantTotinov/PixelForge)**: MIT image processing for .NET, built on SkiaSharp. If you have used ImageSharp, you already know the API, with no license key and no build-time checks. It is safe by default for user uploads: decompression bombs are rejected from the header before any pixel memory is allocated, and EXIF and GPS metadata never reach the output. It runs on Windows, macOS, Debian and Alpine, x64 and arm64, with no native packages to install. On [NuGet](https://www.nuget.org/packages/PixelForge).
- **[UploadGuard](https://github.com/GrantTotinov/UploadGuard)**: secure file uploads for ASP.NET Core from one declarative policy. It detects the real file type from its bytes and looks inside for zip bombs, zip slip, Office macros, PDF JavaScript, SVG scripts and image polyglots, with optional ClamAV scanning and image re-encoding through PixelForge. In its published comparison it handles all 14 test files correctly, where popular file-type detection libraries get 4 and 6. On [NuGet](https://www.nuget.org/packages/UploadGuard).
- **[When Protections Silently Do Not Apply](https://github.com/GrantTotinov/aspnetcore-security-bench)**: a [technical report](https://doi.org/10.5281/zenodo.23822216) and benchmark of ASP.NET Core misconfigurations that switch off antiforgery, rate limiting and CORS while the app runs normally and logs nothing. Each case is verified on .NET 8 and .NET 10. The built-in .NET analyzers, Semgrep and CodeQL detect none of them.
- Also: [AiChatRagSystem](https://github.com/GrantTotinov/AiChatRagSystem), Q&A over your own documents with RAG (.NET 8, React, Ollama), [GrantFoodsMAUI](https://github.com/GrantTotinov/GrantFoodsMAUI), a cross-platform food ordering app in .NET MAUI, and [uni-event-app](https://github.com/GrantTotinov/uni-event-app), a university events app in React Native.

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
