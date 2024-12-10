# AI & GenAI Use Case Generator

## Overview
The **AI & GenAI Use Case Generator** is a Python-based tool designed to generate actionable AI/GenAI use cases and collect relevant resources for a given industry and company. It fetches industry insights, company-specific information, and potential AI/GenAI applications, then consolidates them into a comprehensive markdown report. 

This tool is perfect for professionals, researchers, and businesses exploring the potential of AI in specific domains.

---

## Features
- **Industry Research**: Gathers AI-related insights for the specified industry.
- **Company Analysis**: Analyzes the company’s existing use of AI/ML technologies.
- **Use Case Generation**: Produces actionable AI/GenAI use cases tailored to the company and industry.
- **Resource Collection**: Fetches datasets and other resources relevant to the generated use cases.
- **Markdown & Plain Text Reports**: Creates well-structured markdown and plain text reports for easy sharing.

---

## Requirements

### Software
- Python 3.8 or later
- Streamlit

### Dependencies
Install the required dependencies using:
```bash
pip install -r requirements.txt
```

`requirements.txt` should contain:
```plaintext
requests
streamlit
dataclasses
```

### API Keys
You need valid API keys for the following:
- **Tavily API**: For industry and company research (`TAVILY_API_KEY`)
- **Google Gemini API**: For use case generation (`GEMINI_API_KEY`)

Replace the placeholders in the code with your API keys:
```python
self.api_key = "YOUR_TAVILY_API_KEY"
self.api_key = "YOUR_GEMINI_API_KEY"
```

---

## How to Use

### Running the App
1. Save the code to `app.py`.
2. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```
3. Open the app in your web browser (Streamlit provides a URL).

### Generating a Report
1. Enter the **Company Name** and **Industry** in the app form.
2. Click the **Generate Report** button.
3. Wait for the app to:
   - Fetch research data.
   - Generate use cases.
   - Collect resources.
   - Compile and display the report.

### Download Reports
- The generated reports can be downloaded directly from the app in:
  - **Markdown format**: `AI_GenAI_Proposal.md`
  - **Plain Text format**: `AI_GenAI_Proposal_PlainText.txt`

---

## Project Structure

- `app.py`: Main application file.
- `AI_GenAI_Proposal.md`: Markdown report (auto-generated).
- `AI_GenAI_Proposal_PlainText.txt`: Plain text report (auto-generated).

---

## Limitations
- Requires valid API keys to function.
- Depends on the availability and quality of external API data.
- May encounter rate limits or API errors during heavy use.

---

## Example Workflow
1. Input:
   - Company Name: `Acme Corp`
   - Industry: `Healthcare`
2. Output:
   - Industry overview: `Detailed insights into AI applications in healthcare.`
   - Company overview: `Specifics about Acme Corp's AI/ML initiatives.`
   - AI Use Cases: `5 actionable AI/GenAI applications for Acme Corp in healthcare.`
   - Resources: `Links to datasets, research papers, and tools.`

---



---

## Contributors
- **Pranav Kumbhojkar**
- Contributions are welcome! Please feel free to submit issues or pull requests.

--- 

Enjoy exploring the power of AI and GenAI! 🚀
