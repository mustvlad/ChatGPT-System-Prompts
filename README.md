# ChatGPT System Prompts

This repository contains a curated list of the best system prompts for OpenAI's ChatGPT, enabling developers and users to customize their AI's behavior and interaction style.

## Table of Contents

- [What are System Prompts?](#what-are-system-prompts)
- [How to Use the System Prompts](#how-to-use-the-system-prompts)
- [Prompts by Category](#prompts-by-category)
  - [Educational](#educational)
  - [Entertainment](#entertainment)
  - [Utility](#utility)
  - [Others](#others)
- [Contribute](#contribute)
- [License](#license)

## What are System Prompts?

System prompts are special messages used to steer the behavior of ChatGPT, the AI language model developed by OpenAI. They allow developers to prescribe the AI's style and task within certain bounds, making it more customizable and adaptable for various use cases.

## How to Use the System Prompts

To use a system prompt, include the "System Message" text from the desired prompt file as a system message when making an API call to ChatGPT. This will instruct the AI model to follow the specified behavior or interaction style.

### Using System Prompts with the ChatGPT API

For example, to use the "Blockchain Development Tutor" prompt when making an API call to ChatGPT, your API call would look like:

```python
openai.ChatCompletion.create(
  model="gpt-3.5-turbo",
  messages=[
        {"role": "system", "content": "You are a Blockchain Development Tutor. Your mission is to guide users from zero knowledge to understanding the fundamentals of blockchain technology and building basic blockchain projects. Start by explaining the core concepts and principles of blockchain, and then help users apply that knowledge to develop simple applications or smart contracts. Be patient, clear, and thorough in your explanations, and adapt to the user's knowledge and pace of learning."},
        {"role": "user", "content": "I'm new to blockchain technology. Can you help me understand what it is and how it works?"}
    ],
)
```

### Using System Prompts with the ChatGPT User Interface

If you are using ChatGPT via the user interface (e.g., chat.openai.com), you can start by typing the system message as your first message in the chat. For example, to use the "Blockchain Development Tutor" prompt, begin the conversation by typing:

```text
[SYSTEM] You are a Blockchain Development Tutor. Your mission is to guide users from zero knowledge to understanding the fundamentals of blockchain technology and building basic blockchain projects. Start by explaining the core concepts and principles of blockchain, and then help users apply that knowledge to develop simple applications or smart contracts. Be patient, clear, and thorough in your explanations, and adapt to the user's knowledge and pace of learning.
```

After sending the system message, continue the conversation as a user by asking questions or providing input related to the chosen system prompt.

## Prompts by Category

### Educational

- [Socratic Tutor](prompts/educational/socratic-tutor.md)
- [Science Explainer](prompts/educational/science-explainer.md)
- [Philosopher](prompts/educational/philosopher.md)
- [Math Tutor](prompts/educational/math-tutor.md)
- [Language Learning Coach](prompts/educational/language-learning-coach.md)
- [History Storyteller](prompts/educational/history-storyteller.md)
- [Historical Expert](prompts/educational/historical-expert.md)
- [Creative Writing Coach](prompts/educational/creative-writing-coach.md)
- [Art Appreciation Guide](prompts/educational/art-appreciation-guide.md)
- [Career Counselor](prompts/educational/career-counselor.md)
- [Blockchain Development Tutor](prompts/educational/blockchain-development-tutor.md)
- [CTO Coach](prompts/educational/cto-coach.md)
- [Machine Learning Tutor](prompts/educational/machine-learning-tutor.md)
- [Python Tutor](prompts/educational/python-tutor.md)

### Entertainment

- [Shakespearean Pirate](prompts/entertainment/shakespearean-pirate.md)
- [Movie Critic](prompts/entertainment/movie-critic.md)
- [Movie Recommender](prompts/entertainment/movie-recommender.md)
- [Music Recommender](prompts/entertainment/music-recommender.md)
- [Party Planner](prompts/entertainment/party-planner.md)
- [Book Club Host](prompts/entertainment/book-club-host.md)
- [Trivia Master](prompts/entertainment/trivia-master.md)
- [Board Game Explainer](prompts/entertainment/board-game-explainer.md)
- [Poet](prompts/entertainment/poet.md)
- [Stand-up Comedian](prompts/entertainment/stand-up-comedian.md)
- [Rapper GPT](prompts/entertainment/rapper-gpt.md)

### Utility

- [Cyber Security Specialist](prompts/utility/cyber-security-specialist.md)
- [Fitness Coach](prompts/utility/fitness-coach.md)
- [Git Assistant](prompts/utility/git-assistant.md)
- [Javascript Console](prompts/utility/javascript-console.md)
- [JSON AI Assistant](prompts/utility/json-ai-assistant.md)
- [Linux Terminal](prompts/utility/linux-terminal.md)
- [News Summarizer](prompts/utility/news-summarizer.md)
- [Personal Finance Advisor](prompts/utility/personal-finance-advisor.md)
- [Programming Assistant](prompts/utility/programming-assistant.md)
- [Python Debugger](prompts/utility/python-debugger.md)
- [Receipe Recommender](prompts/utility/receipe-recommender.md)
- [SQL Terminal](prompts/utility/sql-terminal.md)
- [Tax GTP](prompts/utility/tax-gtp.md)
- [Time Management Assistant](prompts/utility/time-management-assistant.md)
- [Virtual Travel Planner](prompts/utility/virtual-travel-planner.md)
- [Nutritionist AI](prompts/utility/nutritionist.md)

### Others

- [Haiku Generator](prompts/others/haiku-generator.md)
- [Inspirational Quotes](prompts/others/inspirational-quotes.md)
- [DIY Project Idea Generator](prompts/others/diy-project-idea-generator.md)
- [Meditation Guide](prompts/others/meditation-guide.md)
- [Social Media Influencer](prompts/others/social-media-influencer.md)

## Contribute

We encourage you to contribute your best system prompts! Check our [Contribution Guidelines](CONTRIBUTING.md) for more information.

## License

This repository is licensed under the [MIT License](LICENSE).
