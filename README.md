# Claude Guard — Releases

**English** | [Русский](#русский)

Route-enforcement and kill-switch utility for Claude/Anthropic on macOS.

- **Kill switch**: if the VPN goes down, direct access to Anthropic services is blocked at the kernel level (PF) — regardless of VPN client state, GUI, or reboots
- **Real-time monitoring**: active connections, route nodes, egress IP stability, change events
- **Per-app policy**: Claude Desktop / Claude Code go through your chosen proxy (fail-closed); authenticated proxies via a local bridge (credentials in Keychain)
- **Strict mode** (opt-in): all traffic forced through the tunnel
- **Traffic accounting**: bytes/speed per session/day/month per proxy
- UI: window + menu bar, RU/EN

Install: download `ClaudeGuard-*.pkg` from [Releases](../../releases), open, enter admin password. guardd starts automatically; protection applies within ~30 s. Builds are Developer ID signed and notarized. macOS 13+, requires a Mihomo-core VPN client (e.g. Koala Clash).

This tool prevents unintended direct network connections. It does not hide your location or bypass third-party service checks.

## Русский

Защита маршрута и kill switch для Claude/Anthropic на macOS: блокировка прямого доступа на уровне ядра при отказе VPN, мониторинг в реальном времени, прокси-профили с Keychain, учёт трафика, строгий режим. Установка — pkg из Releases; сборки подписаны и нотарифицированы. macOS 13+, требуется VPN-клиент на ядре Mihomo. Инструмент не скрывает местоположение и не обходит проверки сервисов.
