---
title: "Event 2"
date: 2026-05-23
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Reflection on “FCAJ Community Day (May 23, 2026)”

### Event purpose

This Community Day focused more strongly on career direction in the AI era, the disciplined use of LLMs, and enterprise-grade AI system design. It also expanded into data analysis, infrastructure cost optimization, and product-thinking.

The main objectives were:

- Updating career perspectives in a fast-changing AI landscape
- Understanding the role of context when using AI tools
- Exploring business data analysis with Amazon Q Business
- Learning how AWS CloudFront helps with cost control and infrastructure protection
- Discovering how enterprise-grade multi-agent systems are designed

### Speakers

- **Nguyen Gia Hung** - Solution Architect, AWS Vietnam, Founder of FCAJ
- **Tinh Truong** - Platform Engineer at Got It
- **Hai Anh** - Engineer at Pacific Vietnam
- **Nguyen Huu Thinh** - DevOps Engineer
- **UTM Morpo Team (Uyen, Thao, Mach)** - Hackathon winning team

### Key highlights

#### 1. Career direction in the AI era

One major point from the event was that AI may lower the cost of building software, but it also increases the need for people who can maintain, operate, optimize, and scale those systems properly. In that sense, roles related to platform engineering and system ownership become even more important.

The speakers emphasized that:

- Degrees and strong fundamentals still matter
- Technical skill alone is not enough without business context
- Students should aim to build real products, not only demos

#### 2. Context and the limitations of LLMs

This part made it clear that AI performs well only when it receives the right context. Without domain knowledge, coding conventions, or business requirements, it can easily generate code that looks convincing but adds little real value.

The event also introduced the idea of an “Internet Puller,” meaning the habit of pulling in random code, tools, or libraries from the internet without understanding them. That habit becomes especially dangerous as projects grow larger.

Another important point was that LLM output is not perfectly stable. Even with low temperature settings, responses can still vary. Because of that, systems built around AI must be prepared for malformed or unreliable output.

#### 3. Business data and cloud infrastructure

The **Amazon Q Business** segment was particularly interesting because it showed that AI support is not limited to coding. When connected to business data sources such as Excel files or internal knowledge bases, an agent can help analyze information and create dashboards without requiring much custom implementation.

The **AWS CloudFront** discussion focused on practical business concerns:

- Better cost optimization with the right usage model
- Reducing the risk of bill spikes
- Improving content delivery efficiency
- Strengthening security around the origin infrastructure

#### 4. Enterprise-grade multi-agent systems

This was the most thought-provoking part for me. The speaker explained that complex problems should not be pushed into a single all-purpose agent. A better approach is to divide responsibilities: one agent for financial analysis, another for market research, another for orchestration, and so on.

That model also requires strict attention to:

- Guardrails
- Clear authorization boundaries
- Audit logging
- Security and compliance requirements

### What I learned

#### Technical mindset

- Optimizing LLMs is not only about prompting, but also about context quality and output-risk management
- Multi-agent systems are useful only when roles and boundaries are designed carefully
- Cloud infrastructure should always be evaluated from the perspectives of performance, security, and cost

#### Work mindset

- A good product is not just something that runs, but something that solves the right business problem
- Infrastructure as Code and controlled change management are essential for serious system ownership
- When time and resources are limited, protecting the core value matters more than chasing too many features

### Applying this to my work

After the event, I identified several concrete actions:

- Use AI more selectively instead of relying on unchecked copy-paste workflows
- Review both LLM inputs and outputs carefully before integrating them into a system
- Learn more deeply about serverless architecture and Infrastructure as Code
- Start feature discussions from business context and expected value, not just technical curiosity

### Event experience

This Community Day felt different from many regular tech talks because it highlighted the gap between building a demo and building something that is actually suitable for enterprise use. I was especially impressed by how strongly the speakers prioritized security, compliance, and business value over the excitement of AI alone.

Another memorable lesson came from the Hackathon-winning team’s discussion about feature creep. It reminded me that doing fewer things well can often be more effective than trying to do too much at once.

#### Some event photos
![Event 2](/images/4-Event/event-2.jpg)

### Supporting evidence for Event 2

![Event 2 registration confirmation email](/images/4-Event/event2/registration-email.png)
*Confirmation email for FCAJ Community Day on May 23, 2026.*

![Event 2 QR ticket](/images/4-Event/event2/ticket-qr.png)
*QR check-in ticket for the event at Bitexco Financial Tower.*

![Event 2 venue overview](/images/4-Event/event2/event-room.png)
*A wide view of the event room and attendees before the session started.*

![Event 2 audience photo](/images/4-Event/event2/audience-photo.png)
*Attendees following one of the technical presentation segments.*

![Proposed Deployment Approach slide](/images/4-Event/event2/deployment-approach-slide.png)
*A presentation slide covering enterprise deployment considerations.*

![Basic Deployment Flow slide](/images/4-Event/event2/deployment-flow-slide.png)
*A slide explaining the basic deployment flow discussed during the workshop.*

![Workshop Exercises slide](/images/4-Event/event2/workshop-exercises-slide.png)
*A slide showing the hands-on exercises included in the event.*

![Whiteboard note from Event 2](/images/4-Event/event2/whiteboard-note.png)
*Key themes highlighted during discussion: Security, Reliability, and Scalability.*

> After this event, I gained a clearer understanding of how AI systems should be built in a more practical and sustainable way, especially for enterprise environments and production-oriented projects.
