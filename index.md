---
layout: page
title: Bayesian Optimization Hackathon for Chemistry and Materials
menu_title: Home
menu_icon: house-door
---
{% assign current_date = 'now' | date: "%Y-%m-%d" %}
{% assign event_start_date = site.event_start_date | date: "%Y-%m-%d" %}
{% assign event_close_date = site.event_close_date | date: "%Y-%m-%d" %}
{% assign registration_opens_date = site.registration_opens_date | date: "%Y-%m-%d" %}
{% assign registration_closes_date = site.registration_closes_date | date: "%Y-%m-%d" %}

{% if current_date < registration_opens_date %}
    {% assign registration_status = 'soon' %}
{% elsif current_date >= registration_opens_date and current_date <= registration_closes_date %}
    {% assign registration_status = 'open' %}
{% else %}
    {% assign registration_status = 'closed' %}
{% endif %}

{% if current_date < event_start_date %}
    {% assign event_status = 'soon' %}
{% elsif current_date >= event_start_date and current_date <= event_close_date %}
    {% assign event_status = 'now' %}
{% else %}
    {% assign event_status = 'over' %}
{% endif %}

{:.secondary}
# {{ site.event_date }}, sponsored by the Acceleration Consortium and Merck KGaA

<div class="aside">
    <h2><i class="bi bi-calendar3"></i> Event timeline</h2>
    <dl>
        {% if registration_status == "soon" or registration_status == "open" or registration_status == "demo" %}
            <dt>{{ site.registration_opens_date }}</dt>
            <dd>
                Applications open for participants<br>
                {% if registration_status == 'open' %}
                    <a href="{{ site.baseurl }}{% link registration.md %}" class="btn">Register now</a>
                {% elsif registration_status == 'closed' %}
                    <a class="btn disabled">Registration has closed</a>
                {% elsif registration_status == 'soon' %}
                    <a class="btn disabled">Registration opens soon</a>
                {% endif %}
            </dd>
        {% endif %}

        <dt>{{ site.registration_closes_date }}</dt>
        <dd>Applications close</dd>

        <dt>{{ site.event_date }}</dt>
        <dd>Hackathon date</dd>
    </dl>
</div>

{% if event_status != "over" %}

With the emergence of new [Bayesian optimization tools for the physical sciences](https://chat.openai.com/share/ac610758-2ac8-4b38-8dd5-25e6c46ad2a6), it is important to understand their strengths and weaknesses, reduce the barrier to use, and adapt them for real-world problems. We will put these tools to the test! Scientists from the Acceleration Consortium and Merck KGaA are hosting a 2-day virtual hackathon on {{ site.event_date }} for researchers to work collaboratively in teams on projects related to Bayesian optimization.

Researchers can propose projects from [a range of topics](_/../projects.md) such as applying algorithms to existing benchmarks, developing new benchmark tasks, creating instructional tutorials, proposing real-world chemistry and materials optimization tasks, and more. After the hackathon, results will be collated and presented in a scholarly article.[<sup>(?)</sup>][faq]{:title="What is required for me to participate in the scholarly article?"} Join us to explore, collaborate, innovate, and contribute to the advancement of Bayesian optimization for the physical sciences! [This opportunity](_/../registration.md)
is open to researchers at all levels who are interested in Bayesian optimization[<sup>(?)</sup>][faq]{:title="Are algorithms other than Bayesian optimization allowed?"} for accelerated discovery in chemistry and materials science. Prior programming experience is not required, but for code-focused projects, we recommend beginner-to-intermediate Python programming experience and basic familiarity with git and GitHub.[<sup>(?)</sup>][faq]{:title="Am I eligible to participate in the hackathon?"} Training and orientation resources are available on the [resources page](_/../resources.md).

## Logistics

The event will take place virtually, using a combination of **video
conferencing** ([virtual Gather space](https://app.gather.town/events/nHv-tpANR6a7kCsPCgqJ)) for meetings and seminars and **discussion forums**
([Discourse](https://accelerated-discovery.discourse.group/), [Slack](https://join.slack.com/share/enQtNjc5MjI1NTI3MDUzMy1lNjZlZWZlMGYxNzA3MTY2N2Q2MDA2ZjNlMDQxZmIyMmZkMmNhZmYyMjhhYWQyODM1NDI0Yjg0MGE4NjI3YTBl)) for ongoing comms.

<!-- [AC Discord](https://discord.gg/gZPKDH3pWU) -->

## Outputs

By the end of the event, in addition to applying and developing algorithms, benchmarks, creating tutorials, describing real-world applications, and other projects, we hope you will have formed new connections, learned new skills, and been inspired with new ideas! We will also be working towards a scholarly article[<sup>(?)</sup>][faq]{:title="What is required for me to participate in the scholarly article?"}, and we hope you will be able to contribute to this effort.

{% else %}

With the completion of a 2-day virtual hackathon hosted by scientists from the Acceleration Consortium and Merck KGaA on {{ site.event_date }}, we thank participants for exploring, collaborating, innovating, and contributing to the advancement of Bayesian optimization for the physical sciences.

During the hackathon, researchers had the opportunity to select or develop Bayesian optimization algorithms and apply them to benchmarking tasks, design new benchmark tasks, create instructional tutorials, describe real-world applications, and more. The results of this collaborative effort will be collated and presented in a scholarly article[<sup>(?)</sup>][faq]{:title="What is required for me to participate in the scholarly article?"}.

Although the event has concluded, the outputs from the hackathon, including applied and developed algorithms, benchmarks, and tutorials, will continue to serve as valuable resources for the research community. Outputs from teams that have opted to release their projects are available at https://github.com/AC-BO-Hackathon. We believe that through this event, new connections have been formed, new skills have been acquired, and new ideas have been inspired.

We want to express our gratitude to all the participants for their contributions, and we look forward to future collaborations in advancing Bayesian optimization in chemistry and materials science.
{% endif %}

## Prizes

{% if event_status != "over" %}

Prizes sponsored by [Matterhorn Studio](https://matterhorn.studio/) will be announced the day after the hackathon for the highest-ranked[<sup>(?)</sup>][faq]{:title="What is expected from me if I act as a judge?"} projects (see project showcase and judging session on Day 2 of [agenda](_/../agenda.md)). Tentative prize tiers are below, and submissions from any project topic are eligible. Each prize will be awarded in the form of a gift card.

| Rank | Prize |
| --- | --- |
| First-ranked | Up to CA$300 gift card per team member (max CA$1000) |
| Second-ranked | Up to CA$150 gift card per team member (max CA$500) |
| Third-ranked | Up to CA$75 gift card per team member (max CA$250) |
| 4th-10th ranked | Up to CA$30 gift card per team member (max CA$100) |

{% else %}
We'd like to congratulate the following teams for their outstanding contributions to the hackathon! The top-ranked[<sup>(?)</sup>][faq]{:title="What is expected from me if I act as a judge?"} projects are as follows:

| Rank | # | Team Name | Project Name |
| --- | --- | --- | --- |
1st | Project 23 | Noisy Nerds | Reliable Surrogate Models of Noisy Data |
2nd | Project 34 | BOMS Prob | Streamlining Material Discovery - Bayesian Optimization in Thermal Fluid Mixtures |
3rd | Project 7 | Surface Science Syndicate | BayBE One More Time - Exploring Corrosion Inhibitors for Materials Design |
4th | Project 5 | KLM | Comparing Bayesian Optimization Methods Across Multiple Hyperparameters Against Simulated "Human" Decision-making |
5th | Project 8 | Molecular Representation | BO for Drug Discovery-What is the role of molecular representation? |
6th | Project 9 | PME No Hikari | Optimizing The CO2 Adsorption Capacity of Metal-Organic Frameworks Using Thompson Sampling |
7th | Project 11 | BlenDS | BlendDS - An intuitive specification of the design space for blends of components |
8th | Project 30 | SERO Opt | Active learning for voltammetry waveform design |
9th | Project 43 | Awesome List | Bayesian Optimization Awesome List |
10th | Project 3 | Sparks Group | Take Your Time - Measuring Optimization Performance as a Function of ACQF Optimizer Runtime |

For a full list of hackathon projects, we encourage you to check out the [projects page](_/../projects.md).

{% endif %}

<!-- ## Sponsors

- [The Acceleration Consortium @ University of Toronto](https://acceleration.utoronto.ca/)
- [Merck KGaA](https://www.emdgroup.com/en) -->

## Hosts

<div style="display: flex; align-items: center; justify-content: center;">
    <a href="https://acceleration.utoronto.ca/">
        <img src="./assets/ac-logo.png" alt="The Acceleration Consortium @ University of Toronto" style="width:400px; margin-right: 20px;">
    </a>
    <a href="https://www.emdgroup.com/en">
        <img src="./assets/emd-vibrant-m-logo.png" alt="Merck KGaA" style="width:300px; margin-left: 20px;">
    </a>
</div>

## Prize Sponsor

<div style="display: flex; align-items: center; justify-content: center;">
    <a href="https://matterhorn.studio/">
        <img src="./assets/matterhorn-studio-sheep-logo.png" alt="Matterhorn Studio" style="width:200px;">
    </a>
</div>

[faq]: {{ site.baseurl }}{% link faq.md %}
