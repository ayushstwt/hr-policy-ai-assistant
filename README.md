# HR Policy AI Assistant

HR Policy AI Assistant is a Spring Boot application built using Spring AI that acts as an internal HR chatbot. It helps employees with HR-related queries such as leave policies, working hours, benefits, and code of conduct.

The assistant is restricted to HR topics using a default system prompt. If a user asks anything outside HR policies, it politely declines.

---

## Key Learnings

- Configuring `ChatClient` as a Spring Bean in the configuration layer  
- Using `defaultSystem()` to restrict AI behavior  
- Understanding the purpose of `defaultUser()`  
- Clean separation between configuration and controller layers  

---

## Project Structure

```
ayshirv.com.hrpolicyaiassistant
│
├── config
│   └── ChatClientConfig.java
│
├── controller
│   └── ChatController.java
```

---

## API Endpoint

**GET** `/api/chat?message=Your Question`

Example:

```
GET /api/chat?message=What is the leave policy?
```

---

## Tech Stack

- Java  
- Spring Boot  
- Spring AI  
- OpenAI  

---

---

This project demonstrates how to build a domain-restricted AI assistant using Spring AI with clean architecture practices.
