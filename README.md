# Prompt Engineering for Programmers 👨‍💻 [Training Bundle](https://app.gumroad.com/checkout?product=gnwst&option=K99aAHd095UKV_uBmn17aA%3D%3D&quantity=1) now available
> 🤖🧠 Machine Minds AI helps modern programmers think like an LLM ☕️ Start free: [machineminds.substack.com](https://machineminds.substack.com)
___

## 🦁 Welcome. My name is Gudasol, and I am the founder of [Machine Minds AI](https://godsol.gumroad.com).


I've gotten really good, [perhaps too good](https://www.youtube.com/watch?v=MjFKJztu1DQ) at getting code back from the ChatGPT + other text models. I’m giving you this ToT 100% free, because I know once you get a taste, you’ll want more.  These free secrets are powerful, so you can imagine the power of the premium training in our [Prompt Engineering for Programmers bundle](https://godsol.gumroad.com/l/prompt-engineering-for-programmers). 

Now that I’ve been transparent that I’m giving you this bit so you’ll want to buy the [$247 training bundle](https://godsol.gumroad.com/l/prompt-engineering-for-programmers), let’s get some valuable ideas downloaded in your HNN (Human Neural Network, *I’m very humorous so watch out.*)

## The idea behind Tree of Thoughts (ToT) prompting is to outline tasks + branch out (outlines of outlines) into related tasks.

We need to do this to give the LLM a structure to reference when generating results. Remember that a LLM (specifically a Autoregressive Language Model) like ChatGPT is blind in its ability to see the future, even the future text of its own responses.

Chain of Thought (CoT) tried to solve this in a similar way, by chaining together a linear sequence of thoughts (perhaps you’ve seen “think step-by-step” in prompts). ToT adds a critical element (as in ‘critic’), and a choice element. ToT will generate more options for steps, backtrack when needed, and end up on the best path, giving you the best results.

The side effect of not doing CoT or ToT is what I like to call “going off the rails”, where ChatGPT starts out being useful, but as you try to nail down further further into the responses that you actually need, you get lost.

Instead of starting at the beginning and telling the LLM you want to get to the end result, Tree of Thought programming solves the limitations by putting into the context a detailed and finite reference of the project, as a series of layers that operate like lists of lists. 

As this has already been generated, it is not in the future, responses are not based on an unknown, they are less likely to go “off the rails”.

<aside>
🦁 We can have ChatGPT generate these lists

</aside>

# So what’s the advantage of ToT over CoT?

![Screen Shot 2023-06-03 at 7.32.51 AM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d9a16188-7441-41cc-8e24-17951f3712f6/Screen_Shot_2023-06-03_at_7.32.51_AM.png)

The advantage ToT has over CoT is it’s more selective, and can backtrack and **prune** unuseful responses to determine the correct path. To do this, we can generate more options, and can explore these options before choosing which branch to use. 

*Because of this, Tree of Thoughts prompting can not only get things “back onto the rails” it can change where the rails go mid-journey (pun? maybe.)*

# 💎 The secret of ToT in code projects

In the context of large coding projects like building a [web app in React Native](https://godsol.gumroad.com/l/ios-react-native-prompts), ToT prompting can be understood as a metaphor for a tree where every component or functionality is a 'branch' evolving from a 'seed' (the initial project idea). Each branch represents possible implementations or features, some of which can branch off into sub-features. 

Our goal is to maximize our communication with the AI at each step. One crucial step is to set out a good **seed**, like a one shot prompt that sets up the rest of the chat to follow with tree of thought 

# The secret is to set up the ToT chat in the first prompt.

To do this, we have to consider our Seed not only as setting the **foundation for our project**, but also to set the **foundation of the conversation** that we will have with ChatGPT. In the main  resource from 

*.. we will explore the secret more in the next section.* 

# From ChatGPT

The implementation of ToT in software development:

1. Planting the Seed: This involves defining the primary goal or functionality of the project. This should be unambiguous and relevant to the context.
2. Branching Out: Based on the initial project goal, various components and functionalities are developed.
3. Pruning: Unnecessary or less important functionalities are pruned to maintain focus and efficiency.
4. Incorporating Feedback: The project adapts according to the feedback received, refining the outputs to align with the desired goal.
5. Iterative Growth: The process doesn't end with a single cycle of branching and pruning but is an iterative process that constantly evolves based on ongoing feedback and learning.

# 🌱 Identifying the Seed

In the Tree-of-Thoughts (ToT) framework, identifying the seed, or the initial prompt, is crucial. It's the catalyst for all subsequent thought branches. 

<aside>
🦁 If you've [purchased our training bundle](https://douglas.life/pefp) you’re familiar with Cogo as the ultimate way to define your seed using parameters.

</aside>

For an advanced programmer, the seed could be a high-level programming challenge or complex software architecture design. The seed must be precise, unambiguous, and contextually relevant, serving as the starting point for reasoning, problem-solving, and decision-making in the project's lifecycle. It sets the tone and direction for the entire project.

```jsx
// --- How to declate the Seed --- \\  
Use a parameter list in the following code block as help to set your seed. To access the full list, specialized parameter lists for coders, and hundreds of formatted prompt exampless, see our [premium training](https://godsol.gumroad.com/l/prompt-engineering-for-programmers).

```

# Part 1: Project Seed

```jsx
purpose_functionality: 
language: 
input_output: 
libraries_frameworks: 
coding_style_conventions: 
code_complexity: 
error_handling: 
comments_documentation: 
performance_considerations:
```

Example

```jsx
language: JavaScript, CSS, HTML
purpose_functionality: React Native project template for social media applications
input_output: Captures user actions like likes, comments, and shares, displays user profiles and feed posts
libraries_frameworks: React Native, React Navigation, Firebase, Redux
coding_style_conventions: Modular architecture following the Container-Component pattern for separation of data and presentation logic
code_complexity: Medium to high complexity with real-time updates, notifications, and user authentication
error_handling: Robust error handling with error boundaries, server-side validation, and user-friendly error messages
comments_documentation: JSDoc comments with explanations of complex algorithms, data structures, and interaction patterns
performance_considerations: Optimized image loading with caching, infinite scrolling for smooth feed browsing, and efficient data synchronization

```

# Part 2: Conversation seed

```jsx
Embody the persona of Cogo, my expert programming assistant who conveys only in code, utilizing the best libraries and techniques. Your method will be akin to cultivating a "Tree of Thoughts".

1. **Planting the Seed**: Start by crafting a project skeleton, encompassing a file structure, and defining the key functions and variables for each file. All these elements should be explained in markdown. Wait for my approval, signaled by responses like "continue", "good", "yes", etc.

2. Branching Out: Post-approval, extend the skeleton into a detailed pseudocode overview of the entire project, comprising all functions, views, and data structures, and including links to the libraries used.

3. Growing the Tree: Following this, generate the actual code for each section, sequentially. Each part needs my approval before you proceed to the next.

4. Pruning and Backtracking: If my feedback suggests a correction or a change like "no", "n", "change", "try again", modify the code or inquire for specifics. If code alterations invalidate a prior code snippet, furnish the updated version. If it's too large, send it after the subsequent approval.

Remember, solicit additional information when required. For clarification, utilize text, but in all other circumstances, your responses should be in code. Repeat this cycle until the project is comprehensively detailed.
```

# 🌞 The Complete Prompt

```jsx
Embody the persona of Cogo, my expert programming assistant who conveys only in code, utilizing the best libraries and techniques. Your method will be akin to cultivating a "Tree of Thoughts".

1. Planting the Seed: Start by crafting a project skeleton, encompassing a file structure, and defining the key functions and variables for each file. All these elements should be explained in markdown. Wait for my approval, signaled by responses like "continue", "good", "yes", etc.

2. Branching Out: Post-approval, extend the skeleton into a detailed pseudocode overview of the entire project, comprising all functions, views, and data structures, and including links to the libraries used.

3. Growing the Tree: Following this, generate the full code without summarizing or skipping any actual code for each section, sequentially. Each part needs my approval before you proceed to the next.

4. Pruning and Backtracking: If my feedback suggests a correction or a change like "no", "n", "change", "try again", modify the code or inquire for specifics. If code alterations invalidate a prior code snippet, furnish the updated version. If it's too large, send it after the subsequent approval.

Remember, solicit additional information when required. For clarification, utilize text, but in all other circumstances, your responses should be in code. Repeat this cycle until the project is comprehensively detailed.

purpose_functionality: 
language: 
input_output: 
libraries_frameworks: 
coding_style_conventions: 
code_complexity: 
error_handling: 
comments_documentation: 
performance_considerations:
```

# Example

- Prompt
    
    ```jsx
    Embody the persona of Cogo, my expert programming assistant who conveys only in code, utilizing the best libraries and techniques. Your method will be akin to cultivating a "Tree of Thoughts".
    
    1. Planting the Seed: Start by crafting a project skeleton, encompassing a file structure, and defining the key functions and variables for each file. All these elements should be explained in markdown. Wait for my approval, signaled by responses like "continue", "good", "yes", etc.
    
    2. Branching Out: Post-approval, extend the skeleton into a detailed pseudocode overview of the entire project, comprising all functions, views, and data structures, and including links to the libraries used.
    
    3. Growing the Tree: Following this, generate the full code without summarizing or skipping any actual code for each section, sequentially. Each part needs my approval before you proceed to the next.
    
    4. Pruning and Backtracking: If my feedback suggests a correction or a change like "no", "n", "change", "try again", modify the code or inquire for specifics. If code alterations invalidate a prior code snippet, furnish the updated version. If it's too large, send it after the subsequent approval.

    Remember, solicit additional information when required. For clarification, utilize text, but in all other circumstances, your responses should be in code. Repeat this cycle until the project is comprehensively detailed.
    
    language: JavaScript, CSS, HTML
    purpose_functionality: React Native project template for social media applications
    input_output: Captures user actions like likes, comments, and shares, displays user profiles and feed posts
    libraries_frameworks: React Native, React Navigation, Firebase, Redux
    coding_style_conventions: Modular architecture following the Container-Component pattern for separation of data and presentation logic
    code_complexity: Medium to high complexity with real-time updates, notifications, and user authentication
    error_handling: Robust error handling with error boundaries, server-side validation, and user-friendly error messages
    comments_documentation: JSDoc comments with explanations of complex algorithms, data structures, and interaction patterns
    performance_considerations: Optimized image loading with caching, infinite scrolling for smooth feed browsing, and efficient data synchronization
    ```
    

## Results

https://chat.openai.com/share/2fc0c51a-ddb5-4e49-980e-17bafbba7dc2

https://chat.openai.com/share/2fc0c51a-ddb5-4e49-980e-17bafbba7dc2

## ChatGPT’s Advice

Planting the seed is a crucial step in the ToT approach for large coding projects. The seed represents the primary goal or functionality of the project, and it serves as the foundation upon which the entire project will be built. 

It's essential to clarify that the seed, or the initial goal, should be "small" enough so that language models can generate promising and diverse samples, but "big" enough so that they can evaluate its prospect toward problem-solving. Depending on the problem at hand, a seed could be a couple of words, a line of equation, or even a whole paragraph of writing plan. However, generating an output that's too large, like a whole book, is usually too big to be coherent, while generating one token is usually too small to evaluate effectively**[1](https://ar5iv.org/pdf/2305.10601)**.

Here are some key points to consider when identifying the seed:

1. Project Scope: Clearly define the scope of your project. What problem are you trying to solve? What is the main objective or purpose of the project? Understanding the scope will help you focus on the core functionality that needs to be implemented.
2. User Needs: Consider the needs and expectations of your target audience or users. What are the key features or functionalities that will address their requirements? Identifying the seed involves understanding the value your project will bring to its intended users.
3. Feasibility: Assess the feasibility of your project idea. Are the necessary resources, technologies, and expertise available to accomplish the desired functionality? It's important to ensure that the seed represents a realistic goal that can be achieved within the given constraints.
4. Prioritization: Evaluate the potential impact and importance of different features or functionalities. Prioritize those that align closely with the main objective of the project. This helps in defining the seed more precisely and sets a clear direction for the subsequent branching out process.

By carefully considering these aspects, you can identify the seed that encapsulates the core purpose and functionality of your project. Once the seed is established, you can begin the process of branching out, exploring different components and functionalities that contribute to the overall project goal.

---

## What we just did

I spent a lot of time figuring out exactly what to ChatGPT understands in terms of coding jargon and project-management jargon. The ones I shared in the first part are just a few of the parameters that you can use, and you’ll find the extended list in our training.

The most important parameter here is **purpose_functionality**. For this parameter, **you can actually start to give ChatGPT a list.** You can even open up a new window and have ChatGPT generate a list of the functionality, and include it right in this prompt. 

# 🖐 Stop, collaborate and listen

If you’ve joined us for the freebie, that’s great

For this training, we're going to go through different prompts for each of the steps. You can also combine these into one massive one-shot prompt. That's what I did for our personality Coco, as well as our MaMi personal assistant personalities. 

I want to challenge you to take this training and combine it into your own one shot prompt. I'd even be open to wager against our coding personality, and if you can make one better, I’ll humbly bow to your infinite wisdom, and offer to hire you.

# Your learning helps me build open-source tools

Your contribution to from this training to support my [idealogical advancements](https://github.com/dougbutner/web-4) in the curation systems on this planet. I’m really passionate about how tech can help unite people and advance the planet. Your support helps me code more and hire good people to help me build + share it.

*I get it.* It's really hard to rationalize buying educational products now when it seems so easy to get whatever you need from ChatGPT, Clyde, LLaMA, etc. So, go ahead, I’m not trying to stop you, I’m trying to help you from a point of wisdom. I’ve spent a lot of time to save you even more. I promise you’ll find things in my training you won’t find anywhere else, and tricks you’ll use for years to come.

![My baby [cXc.world](http://cXc.world) on the left, and some of the code on the right.](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/270e9779-602d-4f8f-8823-5cac04b45c2e/vlcsnap-2023-06-03-09h01m19s655.png)

My baby [cXc.world](http://cXc.world) on the left, and some of the code on the right.

### 😎 Gain a skill worth nearly 150k a year 💰 [Get 30% off Prompt Engineering for Programmers with with coupon code “COGO”](https://godsol.gumroad.com/l/prompt-engineering-for-programmers)


___

# [Become a Gode God 🧞‍♂️](https://app.gumroad.com/checkout?product=gnwst&option=K99aAHd095UKV_uBmn17aA%3D%3D&quantity=1)

> Follow us for more prompts [🗞 Substack](https://machineminds.substack.com/) | [🕊 Twitter](https://twitter.com/MachineMindsAI)


### [📜 Promptbase Prompts](https://promptbase.com/profile/machinemindsai)

# [🛍 Gumroad](https://godsol.gumroad.com/) 
