🛡️ SpectraEYE - Enterprise Observability Platform and Applications Hub
SpectraEYE is a comprehensive enterprise ecosystem designed for observability, operational management, internal collaboration, and data security. Built to function as both a multi-tenant SaaS and an On-Premise solution, SpectraEYE eliminates the fragmentation between operational tools, providing a unified hub of applications for DevOps, support, management, and HR teams.

--------------------------------------------------------------------------------
🧩 The SpectraEYE Ecosystem (Applications & Modules)
The SpectraEYE environment consists of a suite of interconnected platforms, each serving a specific operational role:
1. 👁️ SpectraEYE Core
A comprehensive monitoring and incident management platform designed to ensure high availability and transparency for modern services.

    Advanced Monitoring: Features multi-protocol checks (HTTP, Host Ping, TCP, Keyword Search), Cron job/Heartbeat monitoring with grace periods, and maintenance window handling.
    Incident Lifecycle & Transparency: Manages the full incident workflow (detection to post-mortem), orchestrates team responses with flexible on-call schedules, and communicates system health via public Status Pages.

2. ⚡ SpectraMonitor (Lite)
A powerful multi-tenant SaaS platform with a modern interface, specifically tailored for DevOps teams, MSPs, and SaaS providers.

    Modern Uptime Monitoring: Offers diverse checks including Ping, DNS, TCP/UDP, SSL/TLS expiration alerts, and advanced Playwright browser scenarios.
    Rapid Response: Features global timezone-aware on-call schedules, smart escalation policies, multi-channel notifications (Twilio SMS/Voice, Email), and a Super Admin Console for tenant and license management.

3. 🎧 SpectraServiceDesk
A unified multi-tenant platform for ITSM and Project Management.

    Seamlessly integrates technical support (ticketing workflows, SLA engines, CSAT tracking) with project delivery (tasks, Gantt charts, risk management).
    Features a dedicated Customer Portal for self-service requests and a structured Knowledge Base.

4. 💬 SpectraSocial
An internal social network and digital workplace created for professional enterprise collaboration.

    Centralizes communication through social feeds, 1:1 direct messaging, stories, and event management.
    Drives internal engagement and mobility via dedicated Careers (internal job board) and Marketplace modules.

5. 🎓 SpectraLearn
A comprehensive multi-tenant LMS (Learning Management System) and B2B platform for organizational learning.

    Learning Engine: Delivers educational content including text, video, quizzes, and features native support for SCORM 1.2 and 2004 packages.
    Compliance & Governance: Drives organizational compliance through mandatory course assignments, automated due-date reminders, and automated certificate generation upon completion.
    Social Learning: Boosts user engagement with gamification features, including discussion boards, leaderboards, skill tracking, and peer endorsements.

6. 📊 SpectraSurvey
A multi-tenant "research & operations" platform that bridges feedback collection with digital asset management (DAM).

    Enables the creation of complex surveys with conditional logic, diverse question types, and advanced analytics (NPS, funnels).
    Includes a robust file management layer with folder structures, file versioning, and secure sharing capabilities.

7. 🔒 SpectraVault
A secure platform dedicated to document lifecycle management and compliance visibility.

    Provides controlled storage, file versioning, and auto-delete/retention policies based on organization thresholds.
    Features strict audit logs and controlled file sharing with passwords, expiration dates, and download limits.


--------------------------------------------------------------------------------
⚙️ Architecture & Technology Stack
The SpectraEYE environment relies on a robust architecture designed for performance, multi-tenancy, and Role-Based Access Control (RBAC).

    Frontend: Predominantly built with React (18/19), TypeScript, and Vite. User interfaces are crafted using TailwindCSS, Shadcn/UI, and Radix, while application state is managed by React Query / TanStack Query. (SpectraEYE Core frontend utilizes jQuery and Chart.js).
    Backend: Most applications within the hub (Monitor, ServiceDesk, Social, Learn, Survey, Vault) are powered by Node.js + Express. The foundational SpectraEYE Core platform runs on PHP 8.x using a custom MVP framework.
    Databases & Storage: The ecosystem heavily utilizes MySQL 8.x for relational data and multi-tenant isolation. File storage is handled via local file systems and Supabase integrations.
    Integrations & Real-Time: Features JWT & MFA authentication flows, real-time updates via WebSockets (ws), and notifications powered by SendGrid (Email) and Twilio (SMS/Voice)
