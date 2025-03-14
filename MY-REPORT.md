![GenI-Banner](https://github.com/genilab-fau/genial-fau.github.io/blob/8f1a2d3523f879e1082918c7bba19553cb6e7212/images/geni-lab-banner.png?raw=true)

# {How can prompt engineering techniques be applied to automate the requirement analysis process in the Software Development Lifecycle (SDLC)?
}

1-liner description of your project

<!-- WHEN APPLICABLE, REMOVE THE COMMENT MARK AND COMPLETE
This is a response to the Assignment part of the COURSE.
-->

* Authors: Sai Vardhan Reddy Kasula  
* Academic Supervisor: [Dr. Fernando Koch](http://www.fernandokoch.me)

  
# Research Question 
How can **large language models (LLMs)** and **prompt engineering techniques** be leveraged to automate **requirement analysis** within the **Software Development Lifecycle (SDLC)**, improving accuracy, efficiency, and reducing ambiguity in software engineering?

---
Requirement engineering is a **critical phase** in the **Software Development Lifecycle (SDLC)**, defining system functionalities and constraints before development begins. However, traditional methods of requirement analysis often suffer from:  

1. **Ambiguity & Inconsistency** – Requirements are often vague or misinterpreted, leading to software defects.  
2. **Time-Intensive Manual Processing** – Human analysts must validate, structure, and refine requirements.  
3. **Scalability Challenges** – Large projects require extensive requirement documentation and validation.  

This research explores how **AI-driven prompt engineering techniques**—such as **Zero-shot, Few-shot, Chain-of-Thought (CoT), Meta Prompting, and Template-based prompting**—can **automate** and **enhance** requirement analysis by leveraging **LLMs** like **GPT-3.5-turbo**.

## Arguments

#### What is already known about this topic
### **What is already known about this topic**  
- **AI-driven NLP models** have demonstrated significant advancements in **natural language understanding**, allowing automated interpretation of software requirements.  
- **Prompt engineering** has emerged as a method to fine-tune LLM responses based on structured input formatting.  
- AI models have been successfully applied in **code generation, test case generation, and requirement validation**, but **automated requirement extraction and refinement remain largely unexplored**.  

### **What this research is exploring**  
- Employing **prompt engineering techniques** to **extract, analyze, and refine** software requirements.  
- Developing **a structured methodology** for generating **functional and non-functional requirements** using AI.  
- Exploring how **LLMs** can **reduce ambiguity** in software specifications and improve **requirement validation**.  

### **Implications for practice**  
- **Improved accuracy** – AI-driven requirement analysis reduces human error.  
- **Optimized SDLC processes** – Automation enhances efficiency in software engineering workflows.  
- **Better standardization** – Structured prompt-based extraction ensures consistent requirement documentation.  

---


# Research Method
### **1. Experimental Setup**  
The study involved **iterative experimentation** with various **prompt engineering techniques** to analyze how LLMs process software requirements. The methodology involved:  

- **Dataset:** Manually curated requirements from real-world software projects.  
- **LLM Model:** OpenAI’s **GPT-3.5-turbo API**.  
- **Testing Scenarios:** Applied on **banking, IoT, fitness, SaaS, and e-commerce** domains.  
- **Evaluation Metrics:** **Accuracy, Consistency, and Context Awareness** of responses.

- ### **2. Prompt Engineering Techniques Evaluated**  

| **Prompting Technique** | **Objective** | **Findings** |
|-------------------------|--------------|-------------|
| **Zero-Shot Prompting** | Understanding LLM's ability to infer requirements without context | Generated generic but logically structured outputs. Lacked domain-specific depth. |
| **Few-Shot Prompting** | Providing example-based learning for improved response accuracy | Increased specificity and coherence in structured requirement extraction. |
| **Chain-of-Thought (CoT) Prompting** | Encouraging step-by-step breakdown of complex queries | Improved interpretability and logical flow in requirement refinement. |
| **Meta Prompting** | Enhancing clarity by rephrasing ambiguous queries | Significant reduction in ambiguity. Useful in refining unclear requirements. |
| **Template-Based Prompting** | Enforcing structured response formats | Ensured consistency in requirement extraction across domains. |

---

# Results

### **1. Case Study: Requirement Analysis for an Online Banking System**  

#### **Functional Requirements (Extracted via Prompting)**  
- **User Registration:** Secure authentication with multi-factor verification.  
- **Fund Transfer:** Real-time and scheduled transactions with fraud detection.  
- **Bill Payment:** Integrated with external billing providers.  
- **Secure Messaging:** Encrypted communication between users and the bank.  

#### **Non-Functional Requirements (Identified through AI-Driven Analysis)**  
- **Scalability:** Support for high concurrent user load.  
- **Security:** AES-256 encryption, compliance with banking standards (PCI-DSS).  
- **Reliability:** 99.99% uptime with automatic failover mechanisms.  

#### **Ambiguity Resolution Example**  
**Requirement:** _"The system must support real-time transaction processing."_  
**Challenges Identified:**  
- **Definition of "real-time"** – Immediate vs. batch processing?  
- **Performance benchmarks** – Maximum allowable processing delay?  
- **Failure handling mechanisms** – What happens if a transaction fails?  

By applying **Chain-of-Thought (CoT) Prompting**, we extracted detailed sub-requirements to clarify ambiguities.

  


# Further research
### **2. Case Study: Smart Home IoT System**  

#### **Key Functional Requirements**  
- **Remote Device Control:** Users can control smart devices from mobile applications.  
- **Automation Rules:** Scheduled execution of predefined device actions.  
- **Energy Optimization:** AI-based power consumption monitoring.  

#### **Potential Security Risks Identified Using Meta Prompting**  
- **Unauthorized Access:** Hacking risk mitigation using multi-factor authentication.  
- **Data Privacy:** Secure cloud storage of user preferences.  
- **Interoperability Risks:** Device compatibility across different IoT protocols.  

**Outcome:** By integrating **LLM-driven analysis**, we systematically extracted **security-critical requirements** that would have otherwise been overlooked.

---

## **Discussion & Lessons Learned**  

### **Key Takeaways**  
1. **Prompt engineering significantly enhances requirement extraction accuracy** – LLMs can effectively translate unstructured inputs into structured requirement breakdowns.  
2. **Chain-of-Thought (CoT) and Meta Prompting are particularly effective** – These techniques help in **clarifying ambiguities and refining vague software requirements**.  
3. **Automating requirement analysis reduces manual effort** – AI-driven requirement extraction can streamline SDLC documentation and validation processes.  
4. **Challenges remain in model reliability and scalability** – Some LLM outputs **require human validation** to ensure correctness in complex scenarios.  

### **Future Research Directions**  
- **Fine-tuning domain-specific LLMs** for **software engineering applications**.  
- **Integration of LLMs with Agile workflows** for **real-time requirement tracking**.  
- **Exploring reinforcement learning** to further refine requirement extraction accuracy.  

---

## **Conclusion**  
The project goal which aimed to investigate prompt engineering methods for automating requirement
analysis has been successfully met. After overcoming initial setup challenges of Ollama I moved to
GPT‑3.5‑turbo and performed experimental tests using zero-shot, few-shot, chain-of-thought, meta, and
template-based prompts. The different techniques each demonstrated unique ways to structure inquiries
and direct the model to produce more precise or understandable answers.
The documentation of these experiments revealed that prompt engineering extends beyond creating superior
questions to systematically directing a model's thought process and achieving consistency while enabling
the possibility of automating intricate tasks such as requirement analysis. This research demonstrates that
well-designed prompts enable extraction of detailed and dependable data from large language models which
then can be implemented in practical SDLC applications.
---
