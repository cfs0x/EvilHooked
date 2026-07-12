<h2 align="center">EvilHooked</h2> 

<p align="center">
  <img src="https://github.com/user-attachments/assets/4e9097f6-b51c-4db7-aeb8-8958b73c8f4d" alt="jsdelivr-logo" width="312px" height="512px"/>
  <br>
  <i>
    <br>This is a commercial graphical framework (web control panel) designed to automate, deploy, and manage advanced AitM (Adversary-in-the-Middle) phishing campaigns. The program acts as a visual add-on to the popular Evilginx security tool, complementing it with its own automation modules based on Node.js ( EvilPuppet) and Playwrightto bypass modern corporate security systems (MFA/2FA, Captcha ( different types ) Cloudflare, etc).
</i>
  <br>

Web by [EvilHOOKED](https://t.me/EvilHooked) | follow us on [Twitter](https://twitter.com/cfs0x) | Discord SERVER xCommunity RProxy LAB the [EvilGinx/Modlishka/NodeJS](https://subscord.com/store/1397884713951170610) | Telegram [Contact](https://t.me/cfs0x)

#### Added: We implemented FAKE notifications when working with targeted targets, 
- Installing file extensions inside the session - downloading from both the server and the extension store + the Evil extension itself for capturing browser data.
 
Main modules and functionalities

#Added: ⚡️ PRO UPDATE: BULLETPROOF AUTOMATION FOR EMAIL 


https://github.com/user-attachments/assets/e609fb93-4dd2-4290-8400-da477e75bf15

#### Central hub for monitoring ongoing attacks in real time.

- Metrics Counters: Displays the total number of sessions (Total Sessions), the number of successful compromises with data collection (Captured), unsuccessful attempts (No Capture), and the counter of active users on phishing pages.
- Captured Sessions: An interactive table for managing intercepted sessions with filtering by phishlets and a button for exporting logs to CSV format.
- Geo-Analytics: A built-in interactive world map (Users By Country) distributes victim traffic by country with the ability to filter for different time periods (current/previous month and year).
- Live Capture Feed: A live activity feed for instantly tracking user activity on the target node.

  <img width="2261" height="1177" alt="Screenshot_5" src="https://github.com/user-attachments/assets/67da6f98-fec5-427a-a72b-9580d2642288" />

#### Basic Evilginx Configurations

The interface completely replaces the need to manually edit configuration files via the Linux console.

- Network settings: Manage the primary domain (Domain), external IP address, and ports for DNS (53) and HTTPS (443).
- SSL management: Automatic issuance of Wildcard certificates (Autocert) for dynamic support of any subdomains.
- Infrastructure masking: The Unauth URL setting determines where the user (or the security scanner) will be redirected if they are not authorized or blocked (for example, to a legitimate YouTube video).
- Filtering: Select a blacklist mode (Blacklist Mode: unauth) to filter out unwanted traffic.

<img width="2251" height="1013" alt="Screenshot_8" src="https://github.com/user-attachments/assets/b55e52ca-c8b0-4f95-aef8-4d637a569cc0" />

#### Integration with newsletters (Gophish & Spam)

The module connects the traffic interception infrastructure with email delivery tools.

- Gophish Integration: The panel connects directly to the Gophish server API (Server URL, API Key).
- Campaign Management: Automatically import, launch, and synchronize phishing campaigns.
- Email Templates: Built-in manager for uploading and editing email templates (Spam / Email Templates).

<img width="2245" height="985" alt="Screenshot_19" src="https://github.com/user-attachments/assets/038533fd-81f4-4af5-a1a2-0b99a1cec0a8" />

#### Advanced functionality (PRO mode)
The PRO section transforms the standard Evilginx into a comprehensive platform for conducting complex Red Teaming operations at the Enterprise level.

- Okta PRO Tweaks: A specialized module for bypassing the security of Okta, one of the largest authentication providers. It includes a stealth mode (No - stealth), which removes obvious phishing suffixes from the address bar, and the creation of OIDC redirects.
- PhishForge Scanner (Automatic Generator): an automated scanner of target websites. Allows manual (Manual Login) or headless background (Automatic Background) opening of the Chrome browser directly on the server. This is used for manually solving captchas, bypassing Cloudflare protection, and performing deep web capture. Supports HTTP proxy operation. Creates Phishlets of any complexity with full bypass of all security systems. We write Phishlets for EVILGINX versions 3.x.x (before our modifications).
- EvilPuppet / Playwright: Integration with the Playwright automation engine and a Node.js bridge script. Used as a sidecar to automatically intercept session cookies and instantly transfer them to an external session manager (Session Manager URL) for persistence in the victim's account.
- JS_Inject Library: a tool for injecting arbitrary JavaScript code into the HTML of target pages on the fly. It allows for modification of the DOM tree, forced display of hidden elements (e.g., hidden Okta login forms), spoofing credentials, or collecting additional data from the victim's browser.
- Intercept Rules: a module for creating rules to "short-circuit" (block) HTTP requests before they are sent to the real server. It's used to block security telemetry, antivirus sandboxes, and bots by immediately returning fake 403 errors, custom JSON responses, or 302 redirects.
- Rewrite Rules: a flexible tool for automatically replacing text content or HTTP headers in the response body (response_body) with regular expression support (Regex). Allows you to customize original pages (change phone numbers, instructions, links).
- Flow Engine Overrides: fine-tuning the proxy engine. Includes CORS Credentials management for seamless proxying between different domains, stripping CSS URL Canary links from styles to hide the proxy from security systems, and sending important event notifications via Webhook.
- User-Agent Manager & Help: Manage unique browser identifiers for different phishlets and a built-in interactive help hub for all PRO platform features.

DNS (Wildcard DNS) Allows you to create subdomains on the fly without having to restart the Nginx web server. The Auto DNS on Startup feature automatically sets up DNS records when the panel starts, using the specified internal network adapter (in this example, 172.18.0.2).

#### Flow (Flow Engine Overrides)
Fine-tuning network interactions:

- CORS Credentials (Enabled) — Allows the transfer of cookies and authorization headers between different domains.
- CSS URL Canary (Enabled) — Automatically strips hidden "canary" links from CSS styles, which security systems use to detect phishing proxies.
- Dynamic Host Log — Logs all dynamic client hosts.
- Flow Webhook URL — A field for sending network logs to external SIEM/alert systems.

<img width="2241" height="1160" alt="Screenshot_18" src="https://github.com/user-attachments/assets/96db41e8-a94a-4589-978b-e1afe9bf8848" />

#### Help & Updates
- Help (Pro Feature Reference) — tiled interactive documentation with a reference for all PRO features.
- Updates / Modify — modules for checking Node.js/Playwright versions, updating components in one click, and changing the panel's digital signatures (Modify) to hide software from intrusion detection systems (EDR/NDR).

#### ADVANCED SPAM ENGINE (Phishing Email Generation) 
An advanced email automation module designed for cloning and customizing legitimate corporate notifications.

Full-fledged brand cloning (Company Cloning): 
- The tool allows you to import an original company email (for example, a system notification from Okta, Microsoft 365, or an internal HR system and and others) in one click.
- The engine automatically parses HTML code, pulls in official logos, fonts, and styles, creating a pixel-perfect copy of the original message.

Automatic link substitution: 
- The system automatically scans the imported email, finds all legitimate links, and replaces them with generated target lures (Lures) linked to Evilginx reverse proxy servers.

Randomization and spam filter bypass: 
- An integrated dynamic tag generator allows you to insert unique identifiers, employee names, custom subjects, and invisible text markers to successfully bypass email security systems (SEG/Spam filters).

#### ANTI-DETECT BROWSER AUTOMATION (Session Management)
A unique module for seamless management of compromised accounts without manual data import.

Automatic profile creation: 
- Once the EvilPuppet module successfully intercepts a valid session (MFA cookies and tokens), the platform automatically makes an API call to the integrated anti-detect browser (e.g., AdsPower, Multilogin, Dolphin{anty}).
- The system instantly creates a new, isolated digital profile for that specific victim.

Seamless transfer without cookie manipulation: 
- All intercepted session data, cookies, and the browser's unique digital fingerprint (Canvas, WebGL, WebRTC, User-Agent) are automatically baked into the created profile.

Instant access: 
- The Red Team operator no longer needs to manually copy JSON/Netscape cookies or use third-party extensions.
- Simply launch the generated profile in the anti-detect browser at any time: the target website will immediately open in an authorized state, completely bypassing repeated security checks and the risk of session resets.

#### Full Logging & Audit
A module for total control over the state of the infrastructure, ensuring maximum transparency of actions for analytics.

Server Logs (OS & Infrastructure Logs): 
- Monitor system resources, network interfaces, Docker containers, incoming connections on ports 53 (DNS) and 443 (HTTPS), and attempts to unauthorizedly scan the server itself.
Platform Logs (EPROXY LAB Logs):
- Detailed audit of operator actions within the web panel, recording of changes to settings, JS injection logs, and Playwright automation script execution statuses.

Evilginx Core Logs: 
- Direct output of console logs from the original Evilginx to the web interface. 
- Allows real-time monitoring of the AitM connection establishment process, victim authorization steps, phishlet triggers, and the exact moment of token interception.

#### MULTI-CHANNEL ALERTS (Notification System): 
A module for instantly alerting the team about important stages of compromise.

Telegram Integration: 
- Configure alerts via a Telegram bot.
- The operator receives an instant push notification with details (which phishlet was triggered, the victim's login, and the cookie interception status).

Email Alerts:
- Send critical reports to the team's secure email inboxes for long-term archiving of successful operations.

External Server (Webhook/SIEM): 
- Send structured JSON logs to a remote data collection server or to a corporate SIEM system to record timings as part of legitimate Red Teaming testing.

#### COMMAND & CONTROL SERVER (Teamwork)
A centralized management server that transforms a standalone tool into a fully-fledged platform for information security specialists to collaborate.

Deploy campaigns from a single center: 
- The command server allows you to remotely deploy configurations, launch new phishing campaigns, distribute domains, and manage a pool of proxy servers from a single panel.

Internal Chat and Communication: 
- An integrated communication panel for operators, allowing them to coordinate actions in real time directly within the EPROXY LAB work interface (without the use of external messengers).

File Transfer:
- A secure, protected gateway for exchanging files (phishlet configurations, custom JS scripts, email databases) between Red Team members.

Role-Based Access: 
- The ability to separate roles: for example, Administrator (manages servers and domains), Operator (monitors the dashboard and downloads sessions), and Analyst (studies logs and behavior of security systems).

## Resources
Visit [RProxy LAB](https://rproxylab.gitbook.io/evilginx-lab-by-cfs0x/) for detailed documentation, tutorials, and live examples of RProxy LAB configurations.

## RProxy LAB by cfs0x: Ultimate RProxy and Proxy Powerhouse

Step into the shadows of elite cyber operations with RProxy LAB by cfs0x—a premier Discord community for phishing virtuosos, proxy wizards, and red team operatives. This is your gateway to cutting-edge tools, exclusive training, and a tight-knit network of experts. Subscription unlocks a treasure trove of resources designed to dominate credential harvesting, bypass defenses, and execute flawless social engineering campaigns.

What You Get with Your Subscription:

- Private Phishlets & Mods: Tailored phishlets for Evilginx2, targeting banks, social media, and corporate logins. Custom mods for maximum stealth and scalability.
- SPMT and Mailer Arsenal: High-powered SMTP mailers for mass phishing, with DKIM spoofing and anti-spam evasion. Send undetectable campaigns at scale.
- Evilginx Web Control Dashboard: Enhanced dashboard for Evilginx—manage sessions, route proxies, and capture credentials in real-time with a sleek, intuitive interface.
- Modlishka Upgrades: Advanced Modlishka mods for reverse proxy phishing—SSL stripping, multi-domain support, and custom hooks for seamless attacks.
- Evilpuppet Modules: Pre-built modules for Evilpuppet—automate browsers for credential stuffing, session hijacking, and puppeted ops with precision.
- Node.js Phishing Projects: Full-stack phishing solutions on Node.js—Express backends, React frontends, API-driven data exfil, and obfuscated payloads. Ready-to-deploy with auto-scaling scripts.
- Exclusive Training & Workshops: Hands-on courses on phishing tradecraft, proxy chaining, and red team tactics. From beginner to pro—master the art of deception.

### Red Team Community: Collaborate with seasoned red teamers. Share strategies, troubleshoot ops, and join live phishing simulations. Get real-time mentorship from the best.

### Why Join RProxy LAB?
Elite Tools: Access battle-tested, private resources unavailable in open-source circles.
Expert Network: Connect with a global crew of ethical hackers and pen-testers for knowledge exchange and support.
Continuous Updates: Stay ahead with regular tool drops, mod updates, and cutting-edge techniques.

### Legal Disclaimer:

All tools and resources are provided for ethical and legal use only, such as authorized penetration testing and security research. RProxy LAB by cfs0x and its creators bear no responsibility for misuse, illegal activities, or any consequences arising from improper application of these tools. Users are solely accountable for ensuring compliance with all applicable laws and regulations.

DM to join the elite. Unleash your potential—ethically, ruthlessly, brilliantly.

## Community and Support
Join our community for discussions and support:
- [Discord Server](https://subscord.com/store/1397884713951170610)
- [Issues Page](https://github.com/cfs0x/RProxy-LAB/issues) for bug reports and feature requests.

### Contributing
Contributions are welcome! If you have ideas for improving configurations or adding new templates, please submit a pull request. Ensure all contributions align with the educational and ethical goals of this project.




