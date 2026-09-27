## 🚀 Hi, I'm Ben, the developer behind BFdev.

During my time managing the IT for a small company I was exposed to the way modern systems work—CRMs, calendars, emails, and website stacks. I saw what a mess these systems can be, and how much time and effort the average user puts into managing them.

Data being manually transferred, calendars not syncing, workflows with no error handling... 

So I learned to build robust automations that utilize modern software platforms to enhance productivity.

---

### 💡 My Philosophy

* **Simplicity First:** Systems should be as easy to use, and as easy to understand, as possible.
* **Time Saving Automation:** Repetitive, boring tasks should be automated where possible.
* **Resilient Infrastructure:** Automations should be able to handle failures with minimal disruption to operations.
* **Practical AI:** AI should be implemented in cases such as natural language interpretation, classification, or basic, repeated designs.

*I developed **BFdev** to provide automations built strictly on these pillars.*

---

### 🛠️ Featured Automations

#### 🔄 [Employee Onboarding](https://github.com)
> Taking a simple but boring process and automating it reliably.
* **The Problem:** Employee onboarding may require transferrals of the same data between multiple platforms, taking up time and leaving room for error.
* **The Solution:** Automate an online form to submit the new employee to Microsoft Entra.
* **The Infrastructure:** Built a multi-stage **n8n** workflow triggered by a React form. The input is validated by a backend API, sent to n8n, and written to Entra.
* **Where the Code Is:** Used a backend API in Next.js to act as a gateway to the system and validate the input, followed by custom **n8n Code Nodes (JavaScript)** to validate and transform the data for Entra.
* **What makes it robust?:** Multiple validation steps, a pre-submission check to Entra for duplicate records, and a database table written to on failure using columns corresponding to the active workflow stage.
* **📂 [View Workflow JSON & Code Nodes inside this Repo](https://github.com)**

#### 📊 [Support Request Logging](https://github.com)
> Taking a simple but boring process and automating it reliably.
* **The Problem:** Legacy support systems still in use can clog up inboxes and require manual processing of requests.
* **The Solution:** The input from an online form updates a queue and from there is logged to HubSpot.
* **The Infrastructure:** React form, backend API for validation, n8n backbone including a database table as a source of truth, and a HubSpot ticket pipeline.
* **What makes it robust?:** Initial validation on input through an API acting as a gateway to the system. An n8n backbone uses a data table as a queue, logging successful submissions only to HubSpot to gracefully allow for downstream failures. Includes duplicate checking prior to submission via an API call to HubSpot.

---

### 🚀 Featured Project: BFshop 
> An interactive analytics workspace for eCommerce merchants (Under Construction)
* **Reason for Building:** Most current platforms providing analytics for eCommerce merchants swamp the user in complex dashboards and require heavy data-analysis skills.
* **The Vision:** BFshop will use deterministic analysis of store data, overlaid with an LLM, to provide an easy-to-use, proactive workspace for analyzing store metrics.

---

### 🧰 Tech Stack & Tools

* **Frontend / Frameworks:** Next.js, React, TailwindCSS
* **Backend & Automation:** Node.js, n8n, REST APIs, Webhooks, Databases

---

### 📫 Connect with me

* 🌐 **Website:** [bfdev.com.au](https://benfosterdev.com)
* 🏪 **BFshop:** [bfshop.benfosterdev.com](https://bfshop.benfosterdev.com/)
* 💼 **Company LinkedIn:** [BFdev on LinkedIn](https://www.linkedin.com/company/bfdev/about/?viewAsMember=true)
* 🙍‍♂️ **Personal LinkedIn:** [Ben Foster on LinkedIn](https://www.linkedin.com/in/ben-foster-94394135a/)



