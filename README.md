# Research_agent_phidata_groq

## README

### Overview

This project demonstrates the use of the *Groq model API* to create an advanced AI researcher agent. The agent performs searches, analyzes the results, and generates a comprehensive, engaging report in markdown format. The purpose of this agent is to simulate the work of an experienced researcher, producing professional-quality outputs based on provided topics.

---

### Features

- *AI Researcher Agent:*
  - Powered by the *Groq* model (llama-3.2-11b-vision-preview).
  - Designed to process search results and generate high-quality reports.
  
- *ExaTools Integration:*
  - Performs searches with a specific start date and keyword-based analysis.

- *Dynamic Report Generation:*
  - Outputs markdown-formatted reports structured with:
    - Engaging introductions.
    - Multiple sections with detailed insights.
    - Key takeaways.
    - References for further reading.

- *File Output:*
  - Saves generated reports to a file for future reference (tmp/{message}.md).

---

### Installation

1. *Clone the Repository:*
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. *Install Dependencies:*
   Ensure you have the required Python packages installed:
   ```bash
   pip install phi
   pip install <additional_dependencies_if_any>
   ```

3. *Environment Setup:*
   - Ensure you have access to the *Groq API*.
   - Configure any required API keys or dependencies.

### *Note*: Please add .env file in your working directory and have api key in it of phidata, groq.
---

### Usage

1. *Run the Agent:*
   Execute the script to see the agent in action:
   ```bash
   python <script_name>.py
   ```

2. *Query the Agent:*
   Modify the topic to generate a report on your desired subject:
   python
   ```bash
   agent.print_response("Simulation theory", stream=True)
   ```

   Example topics:
   - "Impact of climate change on biodiversity"
   - "Advancements in quantum computing"

3. *Output File:*
   The generated report will be saved in the tmp/ directory with a filename based on the query.

---

### Report Structure

The generated report follows a consistent format:

markdown
## Engaging Report Title

### Overview
{Brief introduction and engaging hook for the reader}

### Section 1
{Detailed insights and processes for the topic}

... Additional sections as needed ...

### Takeaways
{Key takeaways and conclusions}

### References
- [Reference 1](link)
- [Reference 2](link)
- [Reference 3](link)

- Published on {date} in dd/mm/yyyy


---

### Customization

- *Model Configuration:*
  Modify the Groq model ID in the Agent initialization:
  python
  model=Groq(id="llama-3.2-11b-vision-preview")
  

- *Tool Settings:*
  Adjust ExaTools settings, such as the start_published_date and type:
  python
  tools=[ExaTools(start_published_date="YYYY-MM-DD", type="keyword")]
  

- *Instructions and Output:*
  Customize the agent's behavior by editing the instructions and expected_output parameters.

---

### Example Output

#### Simulation Theory Report

markdown
## Understanding Simulation Theory

### Overview
Simulation theory proposes that our reality might be an artificial simulation, akin to a complex computer program. This concept raises profound philosophical and scientific questions about existence and the nature of reality.

### Section 1: Historical Context
- The concept has roots in ancient philosophy, with parallels to Plato's Allegory of the Cave.
- Modern proponents like Nick Bostrom formalized the theory, suggesting a high probability we live in a simulation.

### Section 2: Scientific Considerations
- Advances in computing and quantum mechanics offer potential evidence.
- Simulations of smaller systems (e.g., protein folding) highlight technological capabilities.

### Takeaways
- Simulation theory encourages exploration of reality's boundaries.
- It challenges our assumptions about existence and scientific discovery.

### References
- [Nick Bostrom's Paper](https://www.simulation-argument.com)
- [Plato's Allegory of the Cave](https://example.com)
- [Quantum Mechanics and Simulations](https://example.com)

- Published on 03/01/2025 in dd/mm/yyyy


---

### Contributing

Contributions are welcome! Feel free to submit pull requests or open issues to suggest improvements.
