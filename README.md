<div align="center">

<img src="https://images.unsplash.com/photo-1461360370896-922624d12aa1?auto=format&fit=crop&w=1600&q=85" alt="Historic museum and classical art" width="100%" />

# 🏛️ Automated Historical Content Publisher

### Bringing the past to your feed — powered by AI.

  An automated content creation and publishing workflow built with **n8n, Google Gemini, and LinkedIn** to generate historical content and      share it on a scheduled basis.

<p>
<img src="https://img.shields.io/badge/n8n-Workflow%20Automation-EA4B71?style=for-the-badge&logo=n8n&logoColor=white" alt="n8n" />
<img src="https://img.shields.io/badge/Google%20Gemini-Generative%20AI-4285F4?style=for-the-badge&logo=google&logoColor=white" alt="Google Gemini" />
<img src="https://img.shields.io/badge/LinkedIn-Content%20Publishing-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</p>

**Explore history. Generate knowledge. Share it automatically.**

</div>

---

## 🏺 The Story Behind the Project

  History is full of fascinating events, discoveries, people, and ideas. Sharing these stories consistently on social media, however, can require time for research, writing, and publishing.
  
  The **Automated Historical Content Publisher** explores how generative AI and workflow automation can simplify this process.
  
  The workflow uses a scheduled trigger to start content generation, Google Gemini to produce historical content, and LinkedIn to publish the generated post.
  
  > **The vision:** Turn historical knowledge into a repeatable, AI-assisted content publishing workflow.

### Workflow Preview

  <img src="https://res.cloudinary.com/dntdfccdk/image/upload/v1792168037/Screenshot_2026-10-16_215628_hoczgk.png" alt="Automated Historical     Content Publisher" width="100%" />

## ✨ What Makes It Special?

  - ⏰ **Scheduled publishing:** Initiates content generation based on the configured schedule.
  - 🧠 **AI-generated content:** Uses Google Gemini to generate historical posts.
  - 🏛️ **History-focused storytelling:** Can be configured to cover historical events, discoveries, people, and civilizations.
  - 🔗 **LinkedIn integration:** Publishes content through the configured LinkedIn node.
  - 🔄 **End-to-end automation:** Connects content generation and publishing in one workflow.
  - 🧩 **Extendable design:** Can be expanded with fact-checking, images, approval steps, and additional content sources.

## ⚙️ Inside the Workflow

### Workflow Architecture

  ```mermaid
  flowchart TD
      A["⏰ Schedule Trigger"] --> B["🏛️ History Generator"]
      C["🧠 Google Gemini Chat Model"] -.-> B
      B --> D["🔵 LinkedIn — Create a Post"]
  
      style A fill:#172554,color:#FFFFFF,stroke:#60A5FA
      style B fill:#78350F,color:#FFFFFF,stroke:#FBBF24
      style C fill:#1D4ED8,color:#FFFFFF,stroke:#93C5FD
      style D fill:#075985,color:#FFFFFF,stroke:#38BDF8
  ```

### How It Works

**01 — Schedule the workflow**

    The Schedule Trigger starts the automation at the configured time or interval.

**02 — Generate historical content**

    The History Generator node uses the connected Google Gemini Chat Model to generate content according to its configured prompt.

**03 — Publish to LinkedIn**

    The LinkedIn Create a Post node publishes the generated content using the configured LinkedIn account and permissions.

**04 — Repeat automatically**

    When the workflow is enabled and correctly configured, it can repeat the process according to the schedule.

## 🛠️ Technology Stack

  | Technology | Purpose |
  |---|---|
  | **n8n** | Visual workflow automation |
  | **Google Gemini Chat Model** | AI-powered historical content generation |
  | **History Generator** | Configured content-generation chain |
  | **LinkedIn integration** | Automated post publishing |
  | **Mermaid** | Workflow diagram in this documentation |

## 🚀 Getting Started

### Prerequisites

  - An n8n account or self-hosted n8n instance.
  - Access to a supported Google Gemini model.
  - Google Gemini credentials configured in n8n.
  - A LinkedIn account and the required authorization for the configured publishing integration.
  - The exported workflow JSON file.

### Installation and Configuration

**Step 1 — Export the workflow**

    Export the workflow from your n8n workspace as a JSON file.

**Step 2 — Import into n8n**

    Import the JSON file into your own n8n workspace.

**Step 3 — Configure Google Gemini**

    Set up the required credentials and verify the model connection.

**Step 4 — Review the History Generator prompt**

    Customize the instructions to specify the historical topic, writing style, post length, and desired format.

**Step 5 — Configure LinkedIn**

    Connect the appropriate LinkedIn account and verify the permissions and target publishing destination supported by your node.

**Step 6 — Test the workflow**

    Run it manually and inspect the generated content before allowing it to publish.

**Step 7 — Enable scheduled execution**

    Once the content and publishing behavior have been verified, activate or publish the workflow according to your n8n version and               configuration.

## 📝 Example Content Ideas

  The workflow prompt can be adapted to generate posts about:
  
  - Ancient civilizations and their achievements.
  - Important historical events and anniversaries.
  - Scientific discoveries and inventions.
  - Influential historical figures.
  - The origins of technologies we use today.
  - Lessons from history that remain relevant.
  - Interesting historical facts and lesser-known stories.
  
  These are suggested topics; the actual output depends on the prompt configured in your History Generator node.

## 🔮 Future Enhancements

  - [ ] Add historical fact verification against reliable sources.
  - [ ] Include source links and references in generated posts.
  - [ ] Generate a relevant visual for each historical story.
  - [ ] Add a human approval step before publishing.
  - [ ] Prevent duplicate historical topics.
  - [ ] Support different post formats and writing styles.
  - [ ] Maintain a publishing history in Google Sheets.
  - [ ] Add error notifications and execution logging.
  - [ ] Generate content based on historical anniversaries.

## 🔐 Security and Responsible AI

  - Never commit API keys, OAuth tokens, or passwords to GitHub.
  - Store credentials in n8n's credential manager.
  - Inspect exported workflow JSON before sharing it.
  - Review historical claims against trustworthy sources.
  - Be transparent about uncertainty when historical details are disputed.
  - Verify generated content before public publication.
  - Follow LinkedIn's terms and the permissions applicable to your integration.
  
## 📚 Learning Outcomes

  This project demonstrates practical exploration of:
  
  - Workflow automation with n8n.
  - Generative AI integration using Google Gemini.
  - Prompt design for content generation.
  - Social media publishing integration.
  - Scheduled execution and workflow testing.
  - Credential security and responsible AI usage.

## 📁 Suggested Repository Structure

  ```text
  automated-historical-content-publisher/
  ├── README.md
  ├── LICENSE
  ├── workflow/
     └── historical-content-publisher.json
  ```

Add the files you actually include in your repository. Check the workflow JSON for sensitive information before uploading it.

## 👨‍💻 About the Creator

  **Kalikowsik**
  
  Aspiring Full Stack Developer | AI & Automation Enthusiast
  
  Exploring practical applications of generative AI and workflow automation through projects that connect intelligent systems with everyday     tasks.
  
  - GitHub: https://github.com/kanithikalikowsik
  - LinkedIn: www.linkedin.com/in/kanithi-kali-kowsik

## 📄 License

  Distributed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

<div align="center">

### History deserves to be remembered — and shared.

**Generated with Google Gemini · Automated with n8n · Published with LinkedIn**

If you find this project interesting, consider giving the repository a ⭐.

</div>
