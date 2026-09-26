# agentic-krishi-ai
==================================================================
KRISHIMITRA AI AGENT — SMART FARMING ADVISORY PLATFORM
==================================================================

PROBLEM STATEMENT
-----------------
Farmers worldwide face severe challenges including unpredictable yield drops,
extreme climate shifts, localized pest outbreaks, and limited access to expert
agricultural guidance. Traditional advisory services are often fragmented, slow,
and lack hyper-local customization.

KrishiMitra AI bridges this gap by deploying an agentic, data-driven smart
farming assistant that delivers real-time, actionable insights directly to
farmers.


PROPOSED SOLUTION & CORE FEATURES
---------------------------------
KrishiMitra leverages Agentic AI and IBM watsonx Orchestrate to provide:

* Autonomous Multi-Agent Systems (Crop, Weather, Pest, Market Agents)
* RAG-Powered Knowledge Retrieval from ICAR/KVK Guidelines
* Multimodal Pest & Leaf Disease Vision Diagnostics
* Real-Time Micro-Weather & Irrigation Scheduling
* Live APMC Mandi Price Analytics & Cost Optimization
* Regional Dialect Voice Assistance via Web Speech API


SYSTEM ARCHITECTURE BLUEPRINT
-----------------------------
[ Client Interface: Web / Voice ]
               │
               ▼
[ IBM watsonx Orchestrate Gateway ]
               │
      ┌────────┴────────┬─────────────────┬────────────────┐
      ▼                 ▼                 ▼                ▼
[ Crop Agent ]  [ Weather Agent ]  [ Pest Agent ]  [ Market Agent ]
      │                 │                 │                │
      ▼                 ▼                 ▼                ▼
[ RAG Engine ]  [ Weather Sensor ] [ Vision AI ]  [ Mandi Database ]


TECHNOLOGY STACK USED
---------------------
* Frontend: HTML5, Tailwind CSS, JavaScript (ES6+), Font Awesome / Lucide Icons
* Agent Orchestration: IBM watsonx Orchestrate (wxoLoader.js)
* AI Model: IBM Granite 4.0 8B Instruct
* Voice Processing: Web Speech API (Speech Recognition & Speech Synthesis)
* External Integrations: Agmarknet APMC Mandi Data, IMD Weather Feeds, Soil Health Cards


IBM WATSONX ORCHESTRATE CONFIGURATION
-------------------------------------
window.wxOConfiguration = {
  orchestrationID: "0087c08433114eae9924a560f1297d20_f2de1c72-0f0c-4743-994c-bd479ef6c5c8",
  hostURL: "https://au-syd.watson-orchestrate.cloud.ibm.com",
  rootElementID: "root",
  deploymentPlatform: "ibmcloud",
  crn: "crn:v1:bluemix:public:watsonx-orchestrate:au-syd:a/0087c08433114eae9924a560f1297d20:f2de1c72-0f0c-4743-994c-bd479ef6c5c8::",
  chatOptions: {
      agentId: "036cc646-f849-47bd-939f-a2783c49b773", 
  }
};


GETTING STARTED / LOCAL SETUP
-----------------------------
1. Clone the repository:
   git clone https://github.com/YOUR_USERNAME/krishimitra-ai-agent.git

2. Navigate into the project folder:
   cd krishimitra-ai-agent

3. Run local server using Python:
   python -m http.server 8000

4. Open browser at:
   http://localhost:8000


FUTURE SCOPE & ROADMAP
----------------------
[Phase 1] Real-Time IoT Soil Sensor Telemetry Sync
[Phase 2] Autonomous Drone Spraying Dispatch & Satellite SAR Radar
[Phase 3] Smart Contract Farmer-to-Buyer Marketplace & Kisan AI Credit Scoring


LICENSE
-------
Distributed under the MIT License.
================================================================================
