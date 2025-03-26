# hex21-cms
Main Content Management System codebase


## Architectural Diagram (Conceptual)

+----------------+     +----------------+     +----------------+
| Content        | --> | Version        | --> | Automation     |
| Authoring      |     | Control (Git)  |     | (GitHub Actions)|
+----------------+     +----------------+     +----------------+
         |                        |
         v                        v
+----------------+       +----------------+
| Metadata       | <---  | Transformation |
| Management     |       | (DITA Toolkit) |
+----------------+       +----------------+
         |                        |
         v                        v
+----------------+       +----------------+
| Front-End      | --->  | Hosting        |
| Rendering      |       | (Vercel/Netlify)|
| (Next.js)      |       +----------------+
+----------------+
