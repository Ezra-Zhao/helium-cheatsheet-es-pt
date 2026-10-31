# Helium 浏览器速查表 | Helium Cheatsheet | Guía rápida de Helium

> 一页看懂 Helium：基于 Chromium 的隐私浏览器——和 Chrome 长得几乎一样，但不盯着你。去 Google 化、默认隐私拉满、内置 uBlock Origin 并保留 Manifest V2，无账号、无同步，配置全存本地。

- 上游项目：[imputnet/helium](https://github.com/imputnet/helium)（2026-10-29 实测 22,159 ★ / 664 forks，117 个 release；GitHub 官方 Octoverse 2026 博客列入社区/独立项目「按贡献者增长最快」前 10）
- 平台：macOS / Windows / Linux
- 本页结构：中文主文 → English → Español → Português

---

Apoyo y más: [GitHub Sponsors](https://github.com/sponsors/Ezra-Zhao) · [Gumroad — plantillas y cuadernos que uso](https://ezraflow28.gumroad.com) · [Ko-fi](https://ko-fi.com/ezra777zhao)

## 它做了什么

| 特性 | 说明 |
|---|---|
| 去 Google 化 | 脱胎于 ungoogled-chromium：底层的 Google 遥测、账号绑定与上报通道先拔干净 |
| 默认隐私配置 | 不用你逐页翻设置：追踪防护等隐私项默认就是收紧的 |
| 内置 uBlock Origin | 出厂自带 uBlock Origin，并**保留 Manifest V2 支持**（广告拦截扩展的完整能力不被阉割） |
| 无账号无同步 | 没有「登录浏览器」这回事，书签、历史、配置全存本地 |
| Helium services | 一层隐私中介：下载扩展、更新过滤清单、浏览器更新、用 !bangs 快捷搜索时请求经它匿名化——外部服务不知道你装了什么、用的是哪个浏览器 |

## 下载一行版

| 平台 | 装法 |
|---|---|
| macOS | 官网下载（自动选对应芯片的包）或 GitHub Releases；装好后自动更新 |
| Windows | 官网下载安装包或 GitHub Releases；自动更新 |
| Linux | GitHub Releases 取对应包（macOS/Linux 是主要开发平台，Linux 版打磨最跟手） |

## 首次设置卡

1. 打开 `helium://setup` 走首次设置向导，别跳过。
2. **默认隐私档 vs 自定义档**：直接选默认隐私档先用起来——它就是为「不想逐项研究设置」的人准备的；明确知道自己要放行什么（比如某个站点的登录态、某类脚本）再进自定义档逐项调。
3. 导入书签：从旧浏览器导出 HTML 再导入即可；密码建议继续放在独立密码管理器里，不要因为换浏览器就全盘搬进浏览器内置存储。

## 和 Chrome / Brave 的一行区别

| | 底子 | 默认追踪 | 账号绑定 | 多余功能 |
|---|---|---|---|---|
| Chrome | Chromium | 默认上报面最大 | 强绑 Google 账号 | 越加越多 |
| Brave | Chromium | 默认收紧，但自带钱包/资讯等自家服务 | 可选 | 自带一堆自家生态功能 |
| Helium | Chromium（ungoogled） | 默认最小化 | **无账号** | 尽量做减法，只留浏览本身 |

同是 Chromium 底子，网页兼容性不用担心；差别全在**默认收集什么、绑不绑账号、塞不塞私货**。

## 诚实标注区

- **仍在 beta**：官方明说可能有意外问题；主力机换用前，先拿它跑一两周日常网站（银行、办公套件、视频会议网页版）确认兼容，再决定要不要全量迁移。
- **平台优先级**：macOS/Linux 是主要开发平台，Windows 版相对跟随节奏，遇到问题先查是否已知 issue。
- **服务层可自托管**：Helium services 的代码全开源，不想用官方中介可以自架；但自托管的匿名化收益只剩「不经过官方」，按自己威胁模型取舍。
- **隐私≠匿名**：浏览器少收集，不等于你的网络层（IP、运营商）看不见你；别把换浏览器当成万能隐身。

---

## English (summary)

Helium (by imputnet, ~22.2k stars as of 2026-10-29; listed in GitHub's Octoverse 2026 fastest-growing community projects) is a Chromium-based privacy browser that looks like Chrome but does not watch you: de-Googled (built on ungoogled-chromium), privacy-tight defaults, uBlock Origin built in with Manifest V2 support kept, no accounts, no sync, all configuration stored locally. A "Helium services" layer anonymizes the unavoidable network calls — extension downloads, filter-list and browser updates, !bang searches — so outside services cannot tell what you run.

Download from the official site (it auto-picks your package) or GitHub Releases; macOS/Windows builds auto-update. First run: walk the `helium://setup` wizard and stay on the default privacy profile unless you know exactly what you want to loosen.

Honest notes: it is still in beta; macOS/Linux are the primary development platforms; the services layer is open source and self-hostable. And a browser that collects less is not full anonymity — your network layer still sees you.

---

## Español (guía rápida — traducción de estudio, pendiente de revisión por un hablante nativo)

Helium (de imputnet, ~22,2 mil estrellas en octubre de 2026; incluido en la lista Octoverse 2026 de GitHub de proyectos comunitarios de mayor crecimiento) es un navegador basado en Chromium que se ve como Chrome pero no te vigila:

- **Sin Google**: construido sobre ungoogled-chromium, sin telemetría ni cuentas de Google.
- **Privacidad por defecto**: la configuración restrictiva viene de fábrica, no tienes que cazar ajustes.
- **uBlock Origin integrado** y con **soporte Manifest V2** intacto.
- **Sin cuentas ni sincronización**: marcadores, historial y ajustes viven solo en tu equipo.
- **Helium services**: una capa intermediaria que anonimiza las llamadas inevitables (descargar extensiones, actualizar listas de filtros y el navegador, búsquedas con !bangs) para que los servicios externos no sepan qué usas.

**Descarga**: desde el sitio oficial (elige tu paquete automáticamente) o GitHub Releases, para macOS, Windows y Linux. La primera vez, abre `helium://setup` y quédate con el perfil de privacidad por defecto salvo que sepas exactamente qué quieres aflojar.

**Frente a Chrome y Brave**: mismo motor Chromium, así que la compatibilidad web no es problema; la diferencia está en qué se recopila por defecto, si te obliga a tener cuenta y cuánto relleno trae. Helium hace resta: solo navegar.

**Notas honestas**: sigue en beta (puede haber sorpresas); macOS y Linux son las plataformas principales de desarrollo; la capa de servicios es de código abierto y autoalojable. Y ojo: que el navegador recopile menos no te vuelve anónimo en la red.

---

## Português (guia rápido — tradução de estudo, aguardando revisão de um falante nativo)

O Helium (do imputnet, ~22,2 mil estrelas em outubro de 2026; incluído na lista Octoverse 2026 do GitHub dos projetos comunitários que mais crescem) é um navegador baseado em Chromium que parece o Chrome, mas não fica vigiando você:

- **Sem Google**: construído sobre o ungoogled-chromium, sem telemetria nem conta do Google.
- **Privacidade por padrão**: a configuração restritiva já vem de fábrica, sem você precisar caçar ajuste por ajuste.
- **uBlock Origin embutido** e com **suporte a Manifest V2** intacto.
- **Sem contas e sem sincronização**: favoritos, histórico e ajustes moram só na sua máquina.
- **Helium services**: uma camada intermediária que anonimiza as chamadas inevitáveis (baixar extensões, atualizar listas de filtros e o navegador, buscas com !bangs) para os serviços externos não saberem o que você usa.

**Download**: pelo site oficial (ele escolhe o pacote certo para você) ou pelo GitHub Releases, para macOS, Windows e Linux. Na primeira vez, abra `helium://setup` e fique no perfil de privacidade padrão, a menos que saiba exatamente o que quer afrouxar.

**Contra Chrome e Brave**: mesmo motor Chromium, então compatibilidade com sites não é problema; a diferença está no que é coletado por padrão, se você é obrigado a ter conta e quanta coisa extra vem junto. O Helium subtrai: só navegar.

**Notas honestas**: ainda está em beta (pode haver surpresas); macOS e Linux são as plataformas principais de desenvolvimento; a camada de serviços é open source e pode ser auto-hospedada. E atenção: o navegador coletar menos não torna você anônimo na rede.

---

## 来源与声明

- 灵感来源 / Source / Fuente / Fonte: [imputnet/helium](https://github.com/imputnet/helium)
- 本仓是个人学习整理：内容用我自己的话总结自上游公开文档，不搬运原文；功能细节以 2026-10-29 的上游 README 与官方文档为准，上游迭代很快，请以官方文档为最终依据。
- 西语、葡语部分为学习译稿，待母语校对。Las secciones en español y portugués son traducciones de estudio pendientes de revisión nativa.
- License: MIT © 2026 Guangyi Zhao
