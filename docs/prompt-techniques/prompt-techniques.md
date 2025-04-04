# Prompt Techniques

This section introduces the fundamental concepts of prompt writing for **Alpha,** especially if you’re new to the idea of giving effective prompts. The goal is to help you communicate effectively so Alpha can generate high-quality, relevant code without unnecessary back-and-forth.&#x20;

{% hint style="info" %}
**What is prompting?**

Prompting refers to the text-based instructions you give to Dualite Alpha to interact with it. Think of it as messages guiding Dualite on what to do.
{% endhint %}

### Understanding how Alpha thinks

We've designed Alpha to minimise the number of prompts to achieve a desired output. He's programmed specifically for frontend web and app development. He already understands how a good frontend codebase is structured. Here are some important points about Alpha.

1. Alpha already knows how to organize a front-end codebase and is aware of the programming language, framework and styling library you’ve chosen while the start.
2. Alpha always uses our default framework templates while creating a new project. Example: React & Tailwind template: [https://github.com/dualiteindia/react-tailwind-template](https://github.com/dualiteindia/react-tailwind-template). Moreover, Alpha is capable to modify these starter files as well based on your requirements or prompts.

{% hint style="info" %}
Prompts and messages are essentially the same thing. We use that interchangeably, preferring the latter for simplicity.
{% endhint %}



### Starting a new project/chat

Here are a few tips for your first prompt while starting up a new chat.

1. State the purpose clearly and concisely and explain your vision to Alpha.
2. Let Alpha build a first version, then add more specific details, constraints and data to enhance the output. State exactly what you want and don’t want.
3. Iterate further based on your requirements.

### Single Shot Prompting.

Alpha is capable to process large and complex instructions in one go. There are cases where we've build great looking dashboards in a single prompts like the following video

{% embed url="https://www.youtube.com/watch?campaign=undefined&feature=youtu.be&medium=undefined&source=undefined&v=j5TRniolelg" %}

The above prompt for this is "Generate a finance dashboard for CEOs to manage their company data"

This approach is great if you're starting from scratch, from idea itself. In such case you should be providing Alpha the information about the goal, purpose and constraints of the application. Alpha may take up some liberty on technical implementation and UI, focusing on achieving your usecase. You can make tweeks with next prompts anytime.

### Iterative Prompts

Iterative (multi step) prompting is required if you've a complex usecase with multiple moving parts. Seperating concerns across prompts is fairly good approach here.

Seperating concerns also gives you more space to explain your custom technical requirements effectively. For example, assuming React with Tailwind as the selected framework.

{% hint style="warning" %}
**DON'T**

Build a wedding dashboard that has 2 pages, Page 1 is a Kanban setup to organise my tasks and also a financial tracker to keep in check of the finance and plan that well . Also integrate the API Specification provided.
{% endhint %}

{% hint style="success" %}
**DO**

* Build me a wedding dashboard which has a Kanban setup to organise my tasks. _(_&#x4F;ptiona&#x6C;_) <**Technical details>** Use a theme config to store my design tokens and import fonts from WebFonts)_
* Now add another page for finance tracking to keep in check of the finance and plan that well. Add bar graphs and pie charts also for this page. _Use Tanstack Router instead of React Router._
* Here is my API specification, _integrate them using a custom hook._
{% endhint %}

Ideally, you should not expect a complete web application following all your intricate in one shot. Focus on getting your desired layout and code structure first. Then keep on prompting to add more specific details and features.&#x20;

{% hint style="info" %}
You should club multiple small to medium changes into a single prompt, but not significantly different and large instructions together.&#x20;



Here's an example of _building a fairly complex application with just 3 prompts:_\
[_https://www.youtube.com/watch?v=mq\_5DMq6D6A_](https://www.youtube.com/watch?v=mq_5DMq6D6A)
{% endhint %}

### Image Prompts

As a user, you can upload images along with your prompt and ask Dualite to create a solution based on them.

There are two key approaches: the first is a straightforward copying method.

{% hint style="info" %}
_After uploading the image:_

Create and build a UI that matches the attached image as close as possible.
{% endhint %}

If you add functionalities on top of an existing image, including describing it, that'll also effectively work as well

{% hint style="info" %}
_After uploading the image:_

Build an app as close as the image provided—a Kanban clone. It should allow adding new cards (tickets), reordering them within a column, and moving them between columns.
{% endhint %}

The second one being inspirational. Suppose you've seen a similar page on web and you want your application to have a similar design theme. In this case you should describe what changes or deflections you expect over the attached image.

### Avoid ambiguity&#x20;

Make sure your prompts are clear and concise.&#x20;

{% hint style="warning" %}
**DON'T**\
Make this website better
{% endhint %}

{% hint style="success" %}
**DO**\
Add a sign-up page with typing fields for username, email, and password and include a submit button. Also enhance the layout by adding some extra whitespacing.
{% endhint %}



### Conclusion

Prompting in Dualite Alpha becomes more effective when you combine these strategies. Happy Coding!























