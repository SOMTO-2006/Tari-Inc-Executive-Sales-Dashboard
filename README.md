Project Overview: Tari Inc. Executive Sales Dashboard
![Main Executive Dashboard](https://github.com/SOMTO-2006/Tari-Inc-Executive-Sales-Dashboard/blob/main/Tari%20DAX%20post.png?raw=true)
The Problem: Friction in Executive Reporting
Tari Inc. possessed a rich foundational dataset of historical sales records (2018–2020), but their leadership team was experiencing significant friction when trying to extract actionable insights. The existing reporting structure was static, visually cluttered, and prone to breaking when cross-filtering across different regions and timeframes. Executives were spending too much time digging for top-line metrics and waiting for analysts to manually calculate Sales Rep performance.

Tari Inc. needed a modern, frictionless Business Intelligence solution that not only provided immediate clarity on historical performance but was structurally engineered to scale with the company into the future.

The Solution: A Behavior-Driven "Remote Control"
To solve this, I architected a fully interactive Power BI dashboard designed around human behavior and executive user experience. By prioritizing clean UX/UI and anchoring critical KPIs in high-visibility zones, the dashboard acts as a seamless remote control for Tari Inc.'s leadership to explore their data dynamically without visual fatigue.

Key Technical Executions
Future-Proofed Data Architecture (Star Schema): Rather than relying on default, auto-generated date tables that bloat file sizes, I built a custom Star Schema data model. I engineered a dynamic, rolling calendar that extends through 2026. This allows Tari Inc. to seamlessly ingest live, modern data tomorrow without needing a developer to rewrite the foundational date logic.

Dynamic DAX Logic & Error Handling: I wrote custom Data Analysis Expressions (DAX) to build a dynamic Sales Rep Leaderboard using RANKX, which instantly recalculates depending on the region or year the executive selects. To ensure the dashboard never breaks during a board meeting, I wrapped all margin and ratio calculations in DIVIDE error-handling logic, replacing jagged "#DIV/0!" errors with clean, blank spaces.

Behavioral UI & Cross-Filtering: Leveraging digital consumer behavior, the most critical KPIs are anchored in the top-left corner. The entire canvas is wired with interactive cross-filtering, eliminating the need for clunky dropdown menus. Heavy, secondary metrics (like Average Order Value) were moved into custom tooltips, appearing only when a user explicitly hovers over a data point to ensure zero screen clutter.

The Business Impact
The final product transformed a static 2018–2020 dataset into a highly scalable, lightning-fast application. Tari Inc. leadership now has a distraction-free environment to instantly identify top performers, track regional growth, and make data-driven decisions with zero cognitive friction.
