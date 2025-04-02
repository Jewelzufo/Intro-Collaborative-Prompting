# **Module 4: Practical Applications**

Welcome to **Module 4** of the **Intro to Advanced Granite Prompting** course! In this module, we’ll explore how to apply advanced prompting techniques to real-world scenarios. We’ll cover **classification tasks**, **mathematical reasoning**, and **customizing prompts** for specific industries or use cases.

---

## **4.1 Classification Tasks**

Classification tasks involve categorizing inputs into predefined classes. Granite 3.2 can be fine-tuned or prompted to excel at these tasks, especially when provided with **classification examples**.

### **4.1.1 Using Classification Examples**
Including examples in the prompt helps the model understand the expected output format and improves accuracy. This is known as **few-shot learning**.

**Example Prompt:**
```
Classify the sentiment of the following reviews as "Positive" or "Negative":

1. Review: "The food was amazing!"
   Sentiment: Positive

2. Review: "The service was terrible."
   Sentiment: Negative

Now classify this review: "The ambiance was great, but the wait time was too long."
```

### **4.1.2 Best Practices**
- **Provide Clear Examples**: Ensure examples are representative of the task.
- **Use Consistent Formatting**: Maintain a consistent structure for inputs and outputs.
- **Test and Iterate**: Experiment with different numbers of examples to find the optimal balance.

**Key Takeaway**: Classification examples improve model accuracy by providing context and structure.

---

## **4.2 Real-World Scenarios**

Granite 3.2’s advanced prompting techniques can be applied to a wide range of real-world scenarios. Here are some examples:

### **4.2.1 Customer Support**
- **Function Calling**: Use tools to retrieve customer information or generate support tickets.
- **Multimodal Prompting**: Combine customer queries with internal documentation to provide accurate responses.

**Example Prompt:**
```
System Prompt: You are a customer support agent with access to the FAQ tool. Use it to answer customer queries.
User Query: How do I reset my password?
<tool_call>{"tool_name": "get_faq", "arguments": {"query": "reset password"}}</tool_call>
```

### **4.2.2 Code Generation**
- **Multimodal Prompting**: Combine natural language instructions with code snippets to generate or explain code.
- **CoT Prompting**: Use step-by-step reasoning to debug or optimize code.

**Example Prompt:**
```
Write a Python function to calculate the factorial of a number.

Example:
```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n-1)
```

Now, optimize this function for large inputs.
```

### **4.2.3 Content Creation**
- **RAG Prompts**: Use external documents to generate informed and accurate content.
- **CoT Prompting**: Break down complex topics into digestible steps for tutorials or explanations.

**Example Prompt:**
```
Write a blog post about the benefits of renewable energy, using the following documents:
[Document 1: "Renewable energy reduces carbon emissions."]
[Document 2: "Solar and wind power are cost-effective."]
```

**Key Takeaway**: Advanced prompting techniques make Granite 3.2 versatile for diverse applications.

---

## **4.3 Customizing Prompts**

Tailoring prompts to specific industries or use cases ensures the model generates relevant and accurate responses.

### **4.3.1 Industry-Specific Prompts**
- **Healthcare**: Use technical terminology and adhere to medical guidelines.
- **Finance**: Incorporate financial jargon and regulatory requirements.
- **Legal**: Ensure responses are precise and compliant with legal standards.

**Example Healthcare Prompt:**
```
System Prompt: You are a medical assistant. Provide responses in line with WHO guidelines.
User Query: What are the symptoms of diabetes?
```

### **4.3.2 Use Case Optimization**
- **Chatbots**: Focus on conversational tone and user engagement.
- **Report Generation**: Emphasize clarity, structure, and data accuracy.
- **Educational Content**: Use simple language and step-by-step explanations.

**Key Takeaway**: Customizing prompts to the context ensures more relevant and effective model outputs.

---

## **Module 4 Hands-On Lab**

### **Lab 4.1: Classification Task**
1. **Objective**: Create a prompt for sentiment classification with examples.
2. **Steps**:
   - Write a prompt with 2-3 examples of positive and negative reviews.
   - Test the prompt with a new review and evaluate the model’s response.

### **Lab 4.2: Real-World Application**
1. **Objective**: Design a prompt for a customer support chatbot.
2. **Steps**:
   - Include a system prompt defining the chatbot’s role.
   - Add a user query and test the response.

### **Lab 4.3: Customized Prompt**
1. **Objective**: Tailor a prompt for a specific industry (e.g., finance).
2. **Steps**:
   - Use industry-specific terminology and guidelines.
   - Test the prompt with a relevant query.

---

## **Module 4 Quiz**

1. **What is the purpose of including classification examples in a prompt?**
   - A) To reduce the model’s response time
   - B) To improve the model’s accuracy by providing context
   - C) To increase the model’s size
   - D) To generate shorter responses

2. **Which technique is best for generating code with Granite 3.2?**
   - A) Function calling
   - B) Multimodal prompting
   - C) CoT prompting
   - D) All of the above

3. **Why is customizing prompts important for industry-specific applications?**
   - A) To ensure the model uses generic language
   - B) To make the model’s responses more relevant and accurate
   - C) To reduce the need for examples
   - D) To simplify the prompt structure

---

**Answers:**
1. B) To improve the model’s accuracy by providing context  
2. D) All of the above  
3. B) To make the model’s responses more relevant and accurate

---

Great job completing **Module 4**! You’ve learned how to apply advanced prompting techniques to real-world scenarios and customize prompts for specific needs. In **Module 5**, we’ll dive into **hands-on labs** to reinforce your skills. See you there!
