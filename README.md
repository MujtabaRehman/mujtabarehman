<!-- ============================ HEADER BANNER ============================ -->
<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=220&section=header&text=Mujtaba%20Rehman&fontSize=60&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=Managed%20Defense%20Analyst%20%7C%20Blue%20Teamer%20%7C%20Automation%20Lover&descAlignY=58&descSize=18" width="100%" alt="Header banner"/>
</div>

<div align="center">
  <img src="https://raw.githubusercontent.com/MujtabaRehman/mujtabarehman/main/images/me.jpg" alt="Mujtaba Rehman" height="200" style="border-radius:50%">
</div>

<h1 align="center">Hi, I'm <a target="_blank" rel="noopener noreferrer">Mujtaba!</a> <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="35" alt="wave"></h1>

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&color=8A2BE2&size=26&center=true&vCenter=true&width=700&height=60&duration=3000&pause=800&lines=%F0%9F%9B%A1%EF%B8%8F+Hunting+threats+across+the+SIEM;%F0%9F%94%8D+Detection+Engineering+%7C+Incident+Response;%F0%9F%A4%96+I+love+to+automate+stuff;%F0%9F%93%A1+Turning+noisy+logs+into+actionable+alerts;%F0%9F%9A%80+Open-Source+Enthusiast;%E2%98%81%EF%B8%8F+Currently+leveling+up+in+Cloud+Security+%26+CTI" alt="Typing headline"/>
</div>

<br>

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=MujtabaRehman&style=for-the-badge&color=8A2BE2&label=PROFILE+VIEWS" alt="profile-views"/>
  <img src="https://img.shields.io/github/stars/MujtabaRehman?label=Stars&style=for-the-badge&color=8A2BE2&logo=github" alt="stars">
  <img src="https://img.shields.io/github/followers/MujtabaRehman?label=Followers&style=for-the-badge&color=8A2BE2&logo=github" alt="followers">
</div>

<br>

<!-- ============================ ABOUT ME ============================ -->
<img align="right" alt="Coding animation" width="420" src="https://raw.githubusercontent.com/MujtabaRehman/mujtabarehman/main/images/coding-boy.gif">

## 🧑‍💻 About Me

```json
{
  "name": "Mujtaba Rehman",
  "role": "Managed Defense Analyst",
  "focus": [
    "Detection Engineering",
    "SIEM Operations",
    "Incident Response",
    "Threat Hunting",
    "Attack Surface Assessments"
  ],
  "mindset": ["Blue Teamer", "Automation Lover", "Break it to defend it"],
  "currently_learning": [
    "Cloud Security",
    "Cyber Threat Intelligence (CTI)",
    "Advanced Threat Research"
  ],
  "hobbies": {
    "Gaming": ["Cricket", "Tekken", "Snooker", "PUBG"]
  }
}
```

<br clear="right"/>

<!-- ============================ SOC TERMINAL ============================ -->
## 🖥️ SOC Terminal

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=16&duration=2500&pause=1000&color=00FF9C&background=0D1117&center=false&vCenter=true&multiline=true&width=760&height=170&lines=%24+whoami;mujtaba+%E2%86%92+blue-team+%7C+detection-engineering+%7C+IR;%24+.%2Fingest+--sources+endpoint%2Cnetwork%2Ccloud%2Cidentity;%5B%2B%5D+logs+normalized.+rules+tuned.+false+positives+down+%E2%9C%94;%24+.%2Fhunt+--hypothesis+%22what+did+the+attacker+do+next%3F%22;%5B%21%5D+alert+triaged+%E2%86%92+incident+contained+%E2%86%92+lessons+learned" alt="SOC terminal animation"/>
</div>

A taste of what I write day to day (KQL for Microsoft Sentinel):

```kusto
// Brute-force followed by a successful sign-in from the same IP
let failures = SigninLogs
| where TimeGenerated > ago(1h) and ResultType != 0
| summarize FailCount = count() by IPAddress, UserPrincipalName
| where FailCount >= 10;
SigninLogs
| where TimeGenerated > ago(1h) and ResultType == 0
| join kind=inner failures on IPAddress, UserPrincipalName
| project TimeGenerated, UserPrincipalName, IPAddress, FailCount
```

<!-- ============================ TECH STACK ============================ -->
## 🛠️ Arsenal

### 🔵 SIEM / EDR / Detection
<p>
  <img src="https://img.shields.io/badge/Microsoft_Sentinel-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" alt="Sentinel"/>
  <img src="https://img.shields.io/badge/Splunk-000000?style=for-the-badge&logo=splunk&logoColor=white" alt="Splunk"/>
  <img src="https://img.shields.io/badge/IBM_QRadar-052FAD?style=for-the-badge&logo=ibm&logoColor=white" alt="QRadar"/>
  <img src="https://img.shields.io/badge/Wazuh-005571?style=for-the-badge&logo=wazuh&logoColor=white" alt="Wazuh"/>
  <img src="https://img.shields.io/badge/CrowdStrike-FC0000?style=for-the-badge&logo=crowdstrike&logoColor=white" alt="CrowdStrike"/>
</p>

### 🔴 Offensive / Assessment
<p>
  <img src="https://img.shields.io/badge/Kali_Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white" alt="Kali"/>
  <img src="https://img.shields.io/badge/Burp_Suite-FF6633?style=for-the-badge&logo=portswigger&logoColor=white" alt="Burp"/>
  <img src="https://img.shields.io/badge/Nmap-4682B4?style=for-the-badge&logo=gnometerminal&logoColor=white" alt="Nmap"/>
  <img src="https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white" alt="Wireshark"/>
</p>

### ⚙️ Automation & Infrastructure
<p>
  <img src="https://skillicons.dev/icons?i=py,bash,powershell,linux,docker,git,github,githubactions,azure&theme=dark" alt="Skills"/>
  <img src="https://img.shields.io/badge/Proxmox-E57000?style=for-the-badge&logo=proxmox&logoColor=white" alt="Proxmox"/>
</p>

<!-- ============================ FOCUS AREAS ============================ -->
## 🎯 What I Do

<table align="center">
  <tr>
    <td align="center" width="25%">🔍<br><b>Detection Engineering</b><br><sub>Rules, use cases, tuning &amp; MITRE ATT&amp;CK mapping</sub></td>
    <td align="center" width="25%">🚨<br><b>Incident Response</b><br><sub>Triage, containment, forensics &amp; reporting</sub></td>
    <td align="center" width="25%">📊<br><b>SIEM Operations</b><br><sub>Log onboarding, parsing, dashboards &amp; health</sub></td>
    <td align="center" width="25%">🌐<br><b>Attack Surface Assessments</b><br><sub>Authorized external testing &amp; exposure review</sub></td>
  </tr>
</table>

<!-- ============================ CONNECT ============================ -->
<div align="center">
  <h3><img src="https://github.com/shariqmalik/shariqmalik/raw/main/images/animation.gif" width="30" height="30" alt=""> Connect with me <img src="https://github.com/shariqmalik/shariqmalik/raw/main/images/animation.gif" width="30" height="30" alt=""></h3>
  <a href="https://www.linkedin.com/in/mujtaba-rehman-241685184/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="https://twitter.com/97_mujtaba" target="_blank">
    <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"/>
  </a>
</div>

<br>

<!-- ============================ STATS ============================ -->
<div align="center">
  <h2>📈 Contribution Activities</h2>

  <a href="https://github.com/MujtabaRehman">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats-eight-alpha-58.vercel.app/api?username=MujtabaRehman&theme=midnight-purple&show_icons=true&hide_border=true">
      <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats-eight-alpha-58.vercel.app/api?username=MujtabaRehman&theme=buefy&show_icons=true&hide_border=true">
      <img height="170" alt="GitHub Stats" src="https://github-readme-stats-eight-alpha-58.vercel.app/api?username=MujtabaRehman&theme=midnight-purple&show_icons=true&hide_border=true"/>
    </picture>
  </a>
  <a href="https://github.com/MujtabaRehman">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-streak-stats-six.vercel.app/?user=MujtabaRehman&theme=midnight-purple&date_format=j%20M%5B%20Y%5D&hide_border=true">
      <source media="(prefers-color-scheme: light)" srcset="https://github-readme-streak-stats-six.vercel.app/?user=MujtabaRehman&theme=buefy&date_format=j%20M%5B%20Y%5D&hide_border=true">
      <img height="170" alt="GitHub Streak" src="https://github-readme-streak-stats-six.vercel.app/?user=MujtabaRehman&theme=midnight-purple&date_format=j%20M%5B%20Y%5D&hide_border=true"/>
    </picture>
  </a>

  <br><br>

  <img alt="Contribution graph" width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=MujtabaRehman&theme=react-dark&bg_color=0D1117&color=8A2BE2&line=8A2BE2&point=FFFFFF&area=true&hide_border=true"/>

  <br><br>

  <img alt="Trophies" src="https://github-profile-trophy.vercel.app/?username=MujtabaRehman&theme=onedark&no-frame=true&no-bg=true&row=1&column=7&margin-w=10"/>
</div>

<!-- ============================ SNAKE ============================ -->
<div align="center">
  <h2>🐍 Snake Eating My Contributions</h2>
  <!-- Requires the workflow in .github/workflows/snake.yml (it creates the "output" branch) -->
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/MujtabaRehman/MujtabaRehman/output/github-contribution-grid-snake-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/MujtabaRehman/MujtabaRehman/output/github-contribution-grid-snake.svg">
    <img alt="Snake animation" src="https://raw.githubusercontent.com/MujtabaRehman/MujtabaRehman/output/github-contribution-grid-snake-dark.svg">
  </picture>
</div>

<!-- ============================ FOOTER ============================ -->
<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=18&center=true&vCenter=true&width=700&height=40&color=8A2BE2&lines=%22Defense+wins+when+detection+never+sleeps.%22" alt="Quote"/>
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=120&section=footer" width="100%" alt="Footer"/>
</div>
