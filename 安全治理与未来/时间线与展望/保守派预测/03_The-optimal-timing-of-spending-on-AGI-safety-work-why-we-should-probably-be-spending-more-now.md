# The optimal timing of spending on AGI safety work; why we should probably be spending more now

**来源**: [https://longtermrisk.org/the-optimal-timing-of-spending-on-agi-safety-work-why-we-should-probably-be-spending-more-now/](https://longtermrisk.org/the-optimal-timing-of-spending-on-agi-safety-work-why-we-should-probably-be-spending-more-now/)

---

# The optimal timing of spending on AGI safety work; why we should probably be spending more now – Center on Long-Term Risk

原文链接: https://longtermrisk.org/the-optimal-timing-of-spending-on-agi-safety-work-why-we-should-probably-be-spending-more-now/

# The optimal timing of spending on AGI safety work; why we should probably be spending more now

29 November 2022
by [Tristan Cook](https://longtermrisk.org/author/tristan-cook/ "Posts by Tristan Cook")

Contents

* [Introduction](#Introduction)
* [A qualitative description of the model](#A_qualitative_description_of_the_model)
  + [Research and influence](#Research_and_influence)
  + [Money](#Money)
  + [Preparedness](#Preparedness)
    - [AGI fire alarm](#AGI_fire_alarm)
  + [Success](#Success)
  + [Solving the model](#Solving_the_model)
* [Results](#Results)
  + [Optimal spending scheduled when varying AGI timelines and difficulty of success](#Optimal_spending_scheduled_when_varying_AGI_timelines_and_difficulty_of_success)
  + [Sensitivity](#Sensitivity)
    - [Discount rate](#Discount_rate)
    - [Growth rate](#Growth_rate)
    - [Current money committed to AGI interventions](#Current_money_committed_to_AGI_interventions)
    - [Diminishing returns](#Diminishing_returns)
    - [Parallel vs serial research](#Parallel_vs_serial_research)
    - [Presence of a fire alarm](#Presence_of_a_fire_alarm)
    - [Substitutability of research and influence](#Substitutability_of_research_and_influence)
* [Discussion](#Discussion)
  + [Some hot takes derived from the model](#Some_hot_takes_derived_from_the_model)
    - [The community’s current spending rate is too low](#The_communitys_current_spending_rate_is_too_low)
    - [The optimal spending schedule is generally 5 to 15% better than the default strategy](#The_optimal_spending_schedule_is_generally_5_to_15_better_than_the_default_strategy)
    - [In most cases, we should not ‘wager’ on long AGI timelines when we believe AGI timelines are short](#In_most_cases_we_should_not_wager_on_long_AGI_timelines_when_we_believe_AGI_timelines_are_short)
  + [Limitations](#Limitations)
    - [Research is endogenous](#Research_is_endogenous)
    - [AGI timelines are independent of our spending schedule](#AGI_timelines_are_independent_of_our_spending_schedule)
    - [Research and capabilities are independent.](#Research_and_capabilities_are_independent)
    - [Diminishing returns, and other features, are constant](#Diminishing_returns_and_other_features_are_constant)
    - [The optimal spending schedule is not always found](#The_optimal_spending_schedule_is_not_always_found)
* [Appendix](#Appendix)
  + [Further limitations](#Further_limitations)
    - [Many inputs are required from the user](#Many_inputs_are_required_from_the_user)
    - [Appreciation of money is continuous and endogenous](#Appreciation_of_money_is_continuous_and_endogenous)
    - [The model only maximises the probability of ‘success’ (with constraints given by keeping money and spending non-negative)](#The_model_only_maximises_the_probability_of_success_with_constraints_given_by_keeping_money_and_spending_non-negative)
  + [Technical description](#Technical_description)
    - [Fire alarm](#Fire_alarm)
    - [Preparedness and success](#Preparedness_and_success)
    - [Solving the model](#Solving_the_model-2)
  + [Model guide](#Model_guide)
  + [Explaining and estimating the model parameters](#Explaining_and_estimating_the_model_parameters)
    - [AI timelines](#AI_timelines)
    - [Discount rate](#Discount_rate-2)
    - [Money](#Money-2)
      * [Starting money](#Starting_money)
      * [Real interest rate](#Real_interest_rate)
    - [Research and influence](#Research_and_influence-2)
      * [Marginal returns to spending](#Marginal_returns_to_spending)
      * [Change in price of the stocks when you have more](#Change_in_price_of_the_stocks_when_you_have_more)
      * [Depreciation of stocks](#Depreciation_of_stocks)
    - [Competition effects](#Competition_effects)
    - [Historical spending on research and influence](#Historical_spending_on_research_and_influence)
    - [Fire alarm](#Fire_alarm-2)
      * [Returns to spending during the fire alarm](#Returns_to_spending_during_the_fire_alarm)
      * [Change in price of the stocks when you have more](#Change_in_price_of_the_stocks_when_you_have_more-2)
      * [Competition during the fire alarm period](#Competition_during_the_fire_alarm_period)
    - [Preparedness and probability of success](#Preparedness_and_probability_of_success)
      * [Preparedness](#Preparedness-2)
      * [Probability of success](#Probability_of_success)
  + [Alternate model](#Alternate_model)
    - [Formalisation](#Formalisation)
    - [Estimating parameters](#Estimating_parameters)
      * [Growth rate](#Growth_rate-2)
      * [Competition factor](#Competition_factor)
      * [Diminishing returns to spending](#Diminishing_returns_to_spending)
      * [Depreciation of the direct work](#Depreciation_of_the_direct_work)
      * [Probability of success](#Probability_of_success-2)
    - [Results](#Results-2)
    - [Limitations](#Limitations-2)
  + [Full results from the nine cases](#Full_results_from_the_nine_cases)
* [Robust spending schedules by Monte Carlo simulation](#Robust_spending_schedules_by_Monte_Carlo_simulation)
  + - [Some notes](#Some_notes)
* [Author contributions](#Author_contributions)
* [Acknowledgements](#Acknowledgements)

*Tristan Cook & Guillaume Corlouer*  
*October 24th 2022*

# Summary

When should funders wanting to increase the probability of AGI going well spend their money? We have created a [tool](https://colab.research.google.com/drive/17f0yTYcFSBihZFd8_N7yRjF2XYJDjvBZ?usp=sharing) to calculate the *optimum spending schedule* and tentatively conclude funders collectively should be spending *at least* 5% of their capital each year on AI risk interventions and in some cases up to 35%.

This is likely higher than the current AI risk community spending rate which is at most 3%[48](#easy-footnote-bottom-48-8199 "<a href=\"https://80000hours.org/2021/07/effective-altruism-growing/\" target=\"_blank\" rel=\"noopener\">Todd (2021) </a>claims 1% donated per year for the whole effective altruism community. The Open Philanthropy project spent <a href=\"https://docs.google.com/spreadsheets/d/1XpWNGyho_kkSkVlMsqnddrhnEYW7MRQBmLX0wITYxGQ/edit?usp=sharing\" target=\"_blank\" rel=\"noopener\">&#36;80m in 2021 on AI risk interventions</a>. In 2021 they <a href=\"https://www.forbes.com/profile/dustin-moskovitz/?sh=9ba79cf1dd34\" target=\"_blank\" rel=\"noopener\">had approximately &#36;17.8b committed</a>. Supposing that at least one sixth of their budget is committed to AI risk interventions, this gives a spending rate of at most 2.6%.  The FTX Future Fund has granted <a href=\"https://docs.google.com/spreadsheets/d/1CI-8rUgjU6s63tUnqCk94KlbojEkyheFiHXliT6dE8M/edit#gid=0\" target=\"_blank\" rel=\"noopener\">around &#36;31m on AI risk interventions</a> since starting over a year ago. Supposing at least one tenth of their budget is committed to AI risk interventions, this gives a spending rate of at most &#36;31m/(<a href=\"https://www.forbes.com/profile/sam-bankman-fried/?sh=2eb301b74449\" target=\"_blank\" rel=\"noopener\">&#36;16,600m </a>/10) = 1.9% per year. For the AI s-risk community, the figure is around 3%."). In most cases, we find that the optimal spending schedule is between 5% and 15% better than the ‘default’ strategy of just spending the interest one accrues and from 15% to 50% better than a naive projection of the community’s spending rate[49](#easy-footnote-bottom-49-8199 "This is true when supposing a 4% constant spending rate, which is an overestimate of current spending but maybe underestimating future spending.").

We strongly encourage users to put their own inputs into the [tool](https://colab.research.google.com/drive/17f0yTYcFSBihZFd8_N7yRjF2XYJDjvBZ?usp=sharing) to draw their own conclusions.

The key finding of a higher spending rate is supported by two distinct models we have created, one that splits spending of capital into research and influence, and a second model  (the ‘alternate model’) that supposes we can spend our stock of things that grow on direct work. We focus on the former with the latter described in the appendix since its output is more obviously action-guiding[50](#easy-footnote-bottom-50-8199 "The second model requires us to split activities into capacity growing and capacity shrinking that increase our probability of success whereas the first model talks concretely about the spending rate of money.").

The table below shows our best guess for the optimal spending schedule using the former model when varying the difficulty of achieving a good AGI outcome and AGI timelines. We keep other inputs, such as diminishing returns to spending and interest rate constant[51](#easy-footnote-bottom-51-8199 "The values chosen are discussed <a href=\"#appendix\" target=\"_blank\" rel=\"noopener\">here</a>.").

|  |  |  |  |
| --- | --- | --- | --- |
|  | *Median AGI arrival* | | |
| *Difficulty of AGI success* | 2030[52](#easy-footnote-bottom-52-8199 "25% AGI by 2027, 50% 2030") | 2040[53](#easy-footnote-bottom-53-8199 "50% AGI by AGI by 2040, 75% by 2060") | 2050[54](#easy-footnote-bottom-54-8199 "50% AGI by 2050, 75% by 2075") |
| Easy[55](#easy-footnote-bottom-55-8199 "The easy case is operationalised by the inputs in the model:  Probability of success if AGI this year = 25%, and <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-df22272e38f87dc51eaee6fe74dba29f_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#108;&#61;&#48;&#46;&#50;&#48;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"61\" style=\"vertical-align: 0px;\"/>. The <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-874263a7b361610077e947dd8ffbfa84_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#108;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"5\" style=\"vertical-align: 0px;\"/> term describes the steepness of the s-shaped curve of success.") | Easy difficulty 2030 median[56](#easy-footnote-bottom-56-8199 "The “break even line” is the maximum rate at which the funder can spend and still have their money increase.") | Easy difficulty 2040 median | Easy difficulty 2050 median |
| Medium[57](#easy-footnote-bottom-57-8199 "Probability of success if AGI this year = 10%, and <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-46f6e759c9eec0c0c6340dd27aa18147_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#108;&#61;&#48;&#46;&#49;&#48;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"61\" style=\"vertical-align: 0px;\"/>") | Medium difficulty 2030 median | Medium difficulty 2040 median | Medium difficulty 2050 median |
| Hard[58](#easy-footnote-bottom-58-8199 "p(success if AGI this year) = 4%, and <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-15916adb4531d9a6d2bd54f57cdaa929_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#108;&#61;&#48;&#46;&#48;&#53;\" title=\"Rendered by QuickLaTeX.com\" height=\"13\" width=\"60\" style=\"vertical-align: 0px;\"/>") | Hard difficulty 2030 median | Hard difficulty 2040 median | Hard difficulty 2050 median |

|  |  |  |  |
| --- | --- | --- | --- |
| ***How much better the optimal spending schedule is compared to the 2%+2% constant spending schedule (within-model lower bound******)[59](#easy-footnote-bottom-59-8199 "This is a lower bound for two reasons: first, there may be spending schedules better than those that we present. Second, we calculate the utility of the 4% strategy for an arbitrarily long time horizon whereas we compute the optimal spending schedules within the year 2100.")*** | | | |
|  | Median AGI | | |
|  | 2030 | 2040 | 2050 |
| Easy | 37.6% | 18.4% | 11.8% |
| Medium | 39.3% | 14.9% | 12.0% |
| Hard | 12.3% | 5.85% | 1.55% |

**Some of the critical limitations of our model include: poorly modelling exogenous research, which is particularly important for those with longer timelines, and many parts of the model - such as diminishing returns - remaining constant over time.**

Further, we find that *robust*spending strategies - those that work in a wide variety of worlds - also support a higher spending rate. We show the results of a Monte Carlo simulation in the appendix[60](#easy-footnote-bottom-60-8199 "<em>Added post-publication on 2022-11-29</em>").

# Introduction

Humanity might be living at a hinge moment in history ([MacAskill, 2020](https://globalprioritiesinstitute.org/william-macaskill-are-we-living-at-the-hinge-of-history/#:~:text=William%20MacAskill%20(Global%20Priorities%20Institute%2C%20Oxford%20University),-GPI%20Working%20Paper&text=In%20the%20final%20pages%20of,dangerous%20and%20decisive%20period...)). This is partly due to the unusually high level of existential risks ([Ord, 2020](https://theprecipice.com/)) and, in particular, the significant probability that humanity will build artificial general intelligence (AGI) in the next decades ([Cotra, 2022](https://www.lesswrong.com/posts/AfH2oPHCApdKicM4m/two-year-update-on-my-personal-ai-timelines)). More specifically, AGI is likely to make up for a large fraction of extinction risks in the present and next decades ([Cotra, 2022](https://www.lesswrong.com/posts/pRkFkzwKZ2zfa3R6H/without-specific-countermeasures-the-easiest-path-to)) and stands as a strong candidate to influence the long-term future. Indeed, AGI might play a particularly important role in the long-term trajectory change of Earth-originating life by increasing the chance of a flourishing future ([Bostrom, 2008](https://nickbostrom.com/utopia)) and reducing the risks of large amounts of disvalue ([Gloor, 2016](https://longtermrisk.org/altruists-should-prioritize-artificial-intelligence/)).

Philanthropic organisations aligned with effective altruism principles such as the FTX Foundation and Open Philanthropy play a crucial role in reducing AI risks by optimally allocating funding to organisations that produce research, technologies and influence to reduce risks from artificial intelligence. Figuring out the optimal funding schedule is particularly salient now with the risk of AI timelines under 10 years ([Kokotajlo, 2022](https://www.lesswrong.com/posts/rzqACeBGycZtqCfaX/fun-with-12-ooms-of-compute)), and the substantial growth in effective altruism (EA) funding roughly estimated at 37% per year from 2015 to 2021 for a total endowment of about 46B$ by then end of 2021 ([Todd, 2021](https://forum.effectivealtruism.org/posts/zA6AnNnYBwuokF8kB/is-effective-altruism-growing-an-update-on-the-stock-of)).

Previous work has emphasised the need to invest now to spend more later due to low discount rates ([Hoeijmakers, 2020](https://forum.effectivealtruism.org/posts/CfLoq8nJBzRARohtQ/the-case-for-investing-to-give-later), [Dickens 2020](https://forum.effectivealtruism.org/posts/3fmcNMrR8cktLnoYk/giving-now-vs-later-for-existential-risk-an-initial-approach)). This situation corresponds to a “patient philanthropist”. Research has modelled the optimal spending schedule a patient philanthropist should follow if they face constant interest rates, diminishing returns and a low discount rate accounting for existential risks ([Trammell, 2021](https://globalprioritiesinstitute.org/wp-content/uploads/Trammell-Dynamic-Public-Good-Provision-under-Time-Preference-Heterogeneity.pdf), [Trammell 2021](https://docs.google.com/document/d/1NcfTgZsqT9k30ngeQbappYyn-UO4vltjkm64n4or5r4/edit)). Extensions of the single provider of public goods model allowed for the rate of existential risks to be time-dependent ([Alaya, 2021](https://forum.effectivealtruism.org/posts/mq7DB72ndm6YGtsoH/optimal-allocation-of-spending-on-existential-risk-reduction)) and to include a trade-off between labour and capital where labour accounts for movement building and direct work ([Sempere, Trammell 2021](https://forum.effectivealtruism.org/posts/FXPaccMDPaEZNyyre/a-model-of-patient-spending-and-movement-building)). Some models also discussed the trade-off between economic growth and existential risks by modelling the dynamics between safety technology and consumption technology with an endogenous growth ([Aschenbrenner, 2020](https://globalprioritiesinstitute.org/leopold-aschenbrenner-existential-risk-and-growth/)) and an exogenous growth model ([Trammell, 2021](https://philiptrammell.com/static/ExistentialRiskAndExogenousGrowth.pdf)).

Without more specific quantitative models taking into account AI timelines, growth in funding, progress in AI safety and the difficulty of building safe AI, previous estimates of a spending schedule of just over 1% per year ([Todd 2021](https://forum.effectivealtruism.org/posts/zA6AnNnYBwuokF8kB/is-effective-altruism-growing-an-update-on-the-stock-of), [MacAskill 2022](https://forum.effectivealtruism.org/posts/cfdnJ3sDbCSkShiSZ/ea-and-the-current-funding-situation)) are at risk of underperforming the optimal spending schedule by as much as 40%.

In this work, we consider a philanthropist or philanthropic organisation maximising the probability of humanity building safe AI. The philanthropist spends money to increase the stock of AI safety research and influence over AI development which translates into increasing the probability of successfully aligning AI or avoiding large amounts of disvalue. Our model takes into account AI timelines, the growth of capital committed to AI safety, diminishing returns in research and influence as well as the competitiveness of influencing AI development. We also allow for the possibility of a fire alarm shortly before AGI arrives. Upon “hearing” the fire alarm, the philanthropist knows the arrival time of AGI and wants to spend all of its remaining money until that time. The philanthropist also has some discount rate due to other existential risks and exogenous research that accelerate safety research.

Crucially, we have coded the model into a [notebook](https://colab.research.google.com/drive/17f0yTYcFSBihZFd8_N7yRjF2XYJDjvBZ?usp=sharing) accompanying this blog post that philanthropists and interested users can run to estimate an optimal spending schedule given their estimates of AI timelines, the difficulty of AI safety, capital growth and diminishing returns. Mathematically the problem of finding the optimal spending schedule translates into an optimal control problem giving rise to a set of nonlinear differential equations with boundary conditions that we solve numerically.

We discuss the effect of AI timelines and the difficulty of AI safety on the optimal spending schedule. Importantly, the optimal spending schedule typically ranges from 5% to 35% per year this decade, certainly above the current typical spending of EA-aligned funders. A funder should follow the most aggressive spending schedule this decade if AI timelines are short (2030) and safety is hard. An intermediate scenario yields a yearly average spending of ~12% over this decade. The optimal spending schedule typically performs between 5 to 15% better than the strategy of spending the endowment’s rate of appreciation and between 18% to 40% better than the current EA community spending at ~3% per year.

# A qualitative description of the model

![](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/1e137ad49ec8970ffdffd5426c5c338b.png)

A diagram of the model. The red arrows above show what we, the funders, can control: the amount of money we spend each year on research and influence. The curved red boxes indicate some of the key inputs. An arrow from A to B indicates that B depends on the value of A.

We suppose that a single funder controls *all* of the community’s funding that is earmarked for AI risk interventions and that they set the spending rate for two types of interventions: *research* and *influence.* The funder’s aim is to choose the spending schedule - how much they spend each year on each intervention - that maximises the probability that AGI goes successfully (e.g. does not lead to an existential catastrophe).

The ‘model’ is a set of equations (described in the appendix) and [accompanying Colab notebook](https://colab.research.google.com/drive/17f0yTYcFSBihZFd8_N7yRjF2XYJDjvBZ). The latter, once given inputs from the user, finds the optimal spending schedule.

## Research and influence

We suppose that any spending is on either *research* or *influence*. Any money we don’t spend is saved and gains interest. As well as investing money in traditional means, the funder is able to ‘invest’ in promoting [earning-to-give](https://forum.effectivealtruism.org/topics/earning-to-give), which historically has been a source of a large fraction of the community’s capital.

We suppose there is a single number for each of the stocks of research and influence describing how much the community has of each[61](#easy-footnote-bottom-61-8199 "We use semi-arbitrary units of ‘quality-adjusted relevant effort units’. We use ‘quality-adjusted’ to imply that an expert's hour of contribution is worth more than a novice’s hour of contribution. We use ‘relevant’ to discount any previously acquired research or influence that is no longer useful. We use ‘effort units’ to mostly account for the time that people have put into working on something.").

Research refers to the community’s ability to make AGI a success given we have complete control over the system (modulo being able to delay its deployment indefinitely). The stock of research contains AI safety technical knowledge, skilled safety researchers, and safe models that we control and can deploy. Influence describes the degree of control we have over the development of AGI, and can include ‘soft’ means such as through personal connections or ‘hard’ means such as passing policy. Both research and influence contribute to the probability we succeed and the user can input the degree to which they are ‘substitutable’.

The equations modelling the time evolution of research and influence have the following features:

* Diminishing marginal returns to spending; the returns to growth in research/influence from each additional unit of spending per year decreases.
* Appreciation or depreciation of research/influence over time. For example, our stock of research could depreciate by becoming less relevant over time as paradigms change and influence could depreciate over time if the AI developers we have influence over become less likely to develop AGI compared to another group.
* The price of one unit of research and influence changes based on how much you already have. For example, having more research may open up multiple parallelizable tracks for people to work on, decreasing the cost of research units. Conversely, once we have more research new researchers must spend increasing time catching up on existing work and so research could become more expensive.
* Influence can become more expensive over time due to competition. As other actors enter the field and also wish to influence AI and the field of AI development itself grows, one unit of spending can result in less influence.

## Money

Any money we don’t spend appreciates. Historically the money committed to the effective altruism movement has grown faster than market real interest rates. The model allows for a variable real interest rate, which allows for the possibility that the growth of the effective altruism community slows.

## Preparedness

We use the term *preparedness at time ![t](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dc427e6c482693df2e8d7ba9edecf38.png "Rendered by QuickLaTeX.com") to describe how ‘ready’ we are if AGI arrived at time ![t.](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/451fec08e4fa9cbcc3e843b9d5df9936.png "Rendered by QuickLaTeX.com") Preparedness is a function of research and influence: the more we have of each the more we are prepared. The user inputs the relative importance of each research and influence as well as the degree they are substitutable.*

### AGI fire alarm

We may find it useful to have money before AGI takeoff, particularly if we have a ‘fire alarm’ period where we know that AGI is coming soon and can spend most of it on last-minute research or influence. The model allows for such last-minute spending on research and influence, and so one’s money indirectly contributes to preparedness.

## Success

The probability of success given AGI arriving in year ![t](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dc427e6c482693df2e8d7ba9edecf38.png "Rendered by QuickLaTeX.com") is an S-shaped function of our preparedness. The model is not fixed to any definition of ‘success’ and could be, but is not limited to, “AGI not causing an existential catastrophe” or “AGI being aligned to human values” or “preventing AI caused s-risk”.

Since we are uncertain when AGI will arrive, the model considers AGI timelines input from the user and takes the integral of the product of {the probability of AGI arriving at time ![t](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dc427e6c482693df2e8d7ba9edecf38.png "Rendered by QuickLaTeX.com")} and {the probability of success at time ![t](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dc427e6c482693df2e8d7ba9edecf38.png "Rendered by QuickLaTeX.com") given AGI at time ![t](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dc427e6c482693df2e8d7ba9edecf38.png "Rendered by QuickLaTeX.com")}.

The model also allows for a discount rate to account for non-AGI existential risks or catastrophes that preclude our research and influence from being useful or other factors.

The funder’s *objective function*, the function they wish to maximise, is the probability of making AGI go successfully.

## Solving the model

The preceding qualitative description is of a collection of differential equations that describe how the numerical quantities of money, research and influence change as a function of our spending schedule. We want to find the spending schedule that maximises the objective function, the *optimal spending schedule*. We do this with tools from [optimal control theory](https://en.wikipedia.org/wiki/Optimal_control)[62](#easy-footnote-bottom-62-8199 "We give a more complete account in the technical description. In short, the solution is given as a numerical solution to an expanded set of differential equations."). We call such a schedule the optimal spending schedule.

# Results

## Optimal spending scheduled when varying AGI timelines and difficulty of success

We first review the table from the start of the post, which varies AGI timelines and difficulty of an AGI success while keeping all other model inputs constant. We stress that the results are based on *our* guesses of the inputs (such as diminishing returns to spending) and encourage people to try the tool out themselves.

|  |  |
| --- | --- |
|  |  |
| Figure caption: Yearly optimal spending schedule averaged over this decade, 2022-2030 (left), and the next, 2030-2040 (right). For each level of AI safety difficulty (easy, medium and hard columns) and each decade we reported the average spending rates in research and influence in % of the funder’s endowment. | |

We consider our best guess for the model’s parameters as given in the appendix (see “[explaining and estimating the model parameters](https://docs.google.com/document/d/1iqzwraiNtcnIomshA0ZvgfzfrTa_QOUZs4Ui1_oXAR8/edit#heading=h.oab3ixvn3i1q)”). We describe the effects of timelines and the difficulty of AI safety on the spending schedule in this decade (2022-2030), the effects being roughly similar in the 2030 decade.

In most future scenarios we observe that the average optimal spending schedule is substantially higher than the current EA spending rate standing at around 1-3% per year. The most conservative spending schedule happens when the difficulty of AI safety is hard with long timelines (2050) with an average spending rate of around 6.5% per year. The most aggressive spending schedule happens when AI safety is hard and timelines are short (2030) with an average funding rate of about 35% per year.

For each level of difficulty and each AI timelines, the average allocation between research and influence looks balanced. Indeed, research and influence both share roughly half of the total spending in each scenario. Looking closer at the results in the appendix (see “[appendix results](https://docs.google.com/document/d/1iqzwraiNtcnIomshA0ZvgfzfrTa_QOUZs4Ui1_oXAR8/edit#heading=h.uan0hhqgctee)”), we observe that influence seems to decrease more sharply than research spending, particularly beyond the 2030 decade. This is likely caused by the sharp increase in the level of competition over AI development making units of influence more costly relative to units of research. Although we want to emphasise that the share of influence and research in the total spending schedule could easily change with different diminishing returns in research and influence parameters.

The influence of AI timelines on the optimal spending schedule varies across distinct levels of difficulty but follows a consistent trend. Roughly, with AI timelines getting longer by a decade, the funder should decrease its average funding rate by 5 to 10%, unless AI safety is hard. If AI safety is easy, a funder should spend an average of ~25% per year for short timelines (2030), down to ~18% per year with medium timelines (2040) and down to ~15% for long timelines (2050). If AI safety difficulty is medium then the spending schedule follows a similar downtrend, starting at about 30% with short timelines down to ~12% with medium timelines and down to 10% with long timelines. If AI safety is hard, the decline in spending from short to medium timelines is sharper, starting at 35% per year with short timelines down to ~8% with medium timelines and down to about 5% with long timelines.

Interestingly, conditioning on short timelines (2030), going from AI safety hard to easier difficulty decreases the spending schedule from ~35% to ~25% but conditioning on medium (204) or long (2050) timelines going from AI safety hard to easier difficulty increases the spending schedule from 6% to 18% and 9% to 15% respectively.

In summary, in most scenarios, the average optimal spending schedule in the current decade typically varies between 5% to 35% per year. With medium timelines (2040) the average spending schedule typically stays in the 10-20% range and moves up to the 20-35% range with short timelines (2030). The allocation between research and influence is balanced.

## Sensitivity

In this section, we show the effect of varying one parameter (or related combination) on the optimal spending schedule. The rest of the inputs are described in the appendix. We stress again that these results are for the inputs we have chosen and encourage you to try out your own.

### Discount rate

Varying just the discount rate we see that a higher discount rate implies a higher spending rate in the present.

|  |  |  |
| --- | --- | --- |
|  |  |  |
| Low discount rate d=0.5\% | Standard d=2\% | High discount rate d=5\% |

### Growth rate

It seems plausible that the community and its capital are likely to be going through an unusually fast period of growth that will level off.[63](#easy-footnote-bottom-63-8199 "The opposite is also plausible if AI risk becomes increasingly salient.") When assuming a lower rate of growth we see that the optimal spending schedule is a lower rate, but still higher than the community’s current allocation. In particular, we should be spending faster than we are growing.

|  |  |  |
| --- | --- | --- |
|  |  |  |
| Highly pessimistic growth rate: 5%  growth rate | Pessimistic growth rate: 10%   current growth decreasing to 5% in the five years.[64](#easy-footnote-bottom-64-8199 "Taking <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-00a6cae91d1aea7ea96fbdc67eec405a_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#100;&#101;&#108;&#116;&#97;&#61;&#48;&#46;&#52;\" title=\"Rendered by QuickLaTeX.com\" height=\"13\" width=\"55\" style=\"vertical-align: 0px;\"/>") | Our guess: 20% current growth  decreasing to 8.5% in the next ten years.[65](#easy-footnote-bottom-65-8199 "Taking <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-0b41139e10dad817ff6b4b70c916cb59_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#100;&#101;&#108;&#116;&#97;&#61;&#48;&#46;&#50;\" title=\"Rendered by QuickLaTeX.com\" height=\"13\" width=\"54\" style=\"vertical-align: 0px;\"/>") |

### Current money committed to AGI interventions

We can compute the change in utility when the amount of funding committed to AI risk interventions changes. This is of relevance to donors interested in the marginal value of different causes, as well as philanthropic organisations that have not explicitly decided the funding for each cause area.

|  |  |  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **Starting money multiplier** | 0.001 | 0.01 | 0.1 | 0.5 | 1 | 1.1 | 1.5 | 10 |
| **Absolute utility** | 0.031[66](#easy-footnote-bottom-66-8199 "We see that even with practically no money we still achieve some utility. This is because both (1) the probability of success is non-zero when we have no research or influence, and (2) we already have some research and influence that will depreciate over time with no further spending.") | 0.044 | 0.092 | 0.219 | 0.317 | 0.332 | 0.386 | 0.668 |
| **Multiple of 100% money utility** | 0.098 | 0.139 | 0.290 | 0.691 | 1 | 1.047 | 1.218 | 2.107 |

A different initial endowment has qualitative effects on the spending schedule. For example, comparing the 10% to 1000% case we see that when we have more money we - unsurprisingly - spend at a much higher rate. This result itself is sensitive to the existing stocks of research and influence.

|  |  |
| --- | --- |
|  |  |
| When we have 10% of our current budget of $4000m | When we have 1000% of our current budget |

The spending schedule is not independent of our initial endowment. This is primarily driven by the S-shaped success function. When we have more money, we can beeline for the steep returns of the middle of the S-shape. When we have less money, we choose to save to later reach this point.

### Diminishing returns

We see that, unsurprisingly, lower diminishing returns to spending suggest spending at a higher rate.

|  |  |  |
| --- | --- | --- |
|  |  |  |
| High diminishing returns[67](#easy-footnote-bottom-67-8199 "<img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-4abd609821299959285720d4fd16cc97_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#101;&#116;&#97;&#95;&#82;&#32;&#61;&#32;&#48;&#46;&#49;&#53;&#44;&#32;&#92;&#101;&#116;&#97;&#95;&#73;&#32;&#61;&#32;&#48;&#46;&#49;\" title=\"Rendered by QuickLaTeX.com\" height=\"17\" width=\"145\" style=\"vertical-align: -4px;\"/>") | Our guess[68](#easy-footnote-bottom-68-8199 "As discussed in the appendix, this is <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-cd345307efbd13ec7279a44948d9b283_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#101;&#116;&#97;&#95;&#82;&#32;&#61;&#48;&#46;&#51;&#32;&#44;&#32;&#92;&#101;&#116;&#97;&#95;&#73;&#32;&#61;&#32;&#48;&#46;&#50;\" title=\"Rendered by QuickLaTeX.com\" height=\"16\" width=\"136\" style=\"vertical-align: -4px;\"/>") | Low diminishing returns[69](#easy-footnote-bottom-69-8199 "<img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-9133bdcbcb070fdb99600df69a834096_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#101;&#116;&#97;&#95;&#82;&#32;&#61;&#48;&#46;&#52;&#53;&#32;&#44;&#32;&#92;&#101;&#116;&#97;&#95;&#73;&#32;&#61;&#32;&#48;&#46;&#51;\" title=\"Rendered by QuickLaTeX.com\" height=\"17\" width=\"146\" style=\"vertical-align: -4px;\"/>") |

### Parallel vs serial research

The constant ![\alpha_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2550f17b97b2268eebea86254d5c25d3.png "Rendered by QuickLaTeX.com") controls whether research becomes cheaper as we accumulate more research (![\alpha_R>0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5f310947514007e9bcd792da57c954bc.png "Rendered by QuickLaTeX.com")) or more expensive (![\alpha_R<0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/ebf40d2028c855b005fcd9dcca69dcf9.png "Rendered by QuickLaTeX.com")). The former could describe a case where an increase in research leads to the increasing ability to parallelize research or break down problems into more easily solvable subproblems. The latter could describe a case where an increase in research leads to an increasingly bottlenecked field, where further progress depends on solving a small number of problems that are only solvable by a few people.

|  |  |  |
| --- | --- | --- |
|  |  |  |
| Research is highly serial (\alpha_R=-0.5) | Default (\alpha_R=0) | Research is highly parallelizable (\alpha_R=0.5) |

We see that in a world where research is either highly serial or parallelizable, we should be spending at a higher rate than if it is, on balance, neither. The *parallelizable result* is less surprising than the *serial* result, which we plan to explore in later work.

A more nuanced approach would use a function ![\alpha_R(R(t))](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/c7c0e9185362c4901913e31268c4cae7.png "Rendered by QuickLaTeX.com") such that the field can become more or less bottlenecked as it progresses and the price of research changes accordingly.

### Presence of a fire alarm

Using our parameters, we find the presence of a fire alarm greatly improves our prospects and, perhaps unexpectedly, pushes the spending schedule upwards. This suggests it is both important to be able to correctly identify the point at which AGI is close and have a plan for the post-fire alarm period.

|  |  |  |
| --- | --- | --- |
|  |  |  |
| **No fire alarm**. | **Short fire alarm**: funders spend 10% of one’s money over six months. In this  case, we get 36% more utility than no fire alarm. | **Long fire alarm**: funders spend 20% of one’s money over one year. In this case, we get 56% more utility than no fire alarm. |

### Substitutability of research and influence

Increasing substitutability means that one (weight adjusted[70](#easy-footnote-bottom-70-8199 "This weight-adjusted is the <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-2afeb87159a4918337409f4bf56d689a_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#103;&#97;&#109;&#109;&#97;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"10\" style=\"vertical-align: -4px;\"/> term in the <a href=\"https://en.wikipedia.org/wiki/Constant_elasticity_of_substitution\" target=\"_blank\" rel=\"noopener\">constant elasticity of substitution function</a>")) unit of research can be replaced by closer to one unit of influence to have the same level of preparedness[71](#easy-footnote-bottom-71-8199 "This is done by increasing <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-acdcb3ab7c66c6fb178814c3cf9681a5_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#114;&#104;&#111;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"9\" style=\"vertical-align: -4px;\"/> up to 1.").

Since, by our choice of inputs, we already have much more importance-adjusted research than influence[72](#easy-footnote-bottom-72-8199 "This is due to our choice of <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-2afeb87159a4918337409f4bf56d689a_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#103;&#97;&#109;&#109;&#97;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"10\" style=\"vertical-align: -4px;\"/>"), in the case where they are very poor substitutes we must spend at a high rate to get influence.

When research and influence are perfect substitutes since research is ‘cheaper’[73](#easy-footnote-bottom-73-8199 "In the sense that (1) it depreciates at a lower rate (2) there are lower diminishing marginal returns.") with our chosen inputs the optimum spending schedule suggests that nearly spending should be on research[74](#easy-footnote-bottom-74-8199 "At a high enough spending rate one marginal unit of influence is cheaper than one marginal unit of influence due to diminishing marginal returns").

|  |  |  |  |
| --- | --- | --- | --- |
|  |  |  |  |
| Research and influence are *very* poor substitutes[75](#easy-footnote-bottom-75-8199 " We take <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-29e26d1af3c08acab86fea398051bcc8_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#114;&#104;&#111;&#61;&#45;&#49;&#48;\" title=\"Rendered by QuickLaTeX.com\" height=\"16\" width=\"65\" style=\"vertical-align: -4px;\"/>") | Research and influence are poor substitutes[76](#easy-footnote-bottom-76-8199 "We take <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-f68135cc279bfafa80a1a256caf37edd_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#114;&#104;&#111;&#32;&#61;&#32;&#48;&#46;&#48;&#48;&#49;\" title=\"Rendered by QuickLaTeX.com\" height=\"16\" width=\"73\" style=\"vertical-align: -4px;\"/>") | Standard case[77](#easy-footnote-bottom-77-8199 "This has <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-7d49ef5fe48eaaa3c8f673eef6a813d6_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#114;&#104;&#111;&#61;&#48;&#46;&#51;\" title=\"Rendered by QuickLaTeX.com\" height=\"16\" width=\"56\" style=\"vertical-align: -4px;\"/>") | Research and influence are perfect substitutes[78](#easy-footnote-bottom-78-8199 "This is <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-396264571be5f38a3efb1ebd1148a277_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#114;&#104;&#111;&#61;&#49;\" title=\"Rendered by QuickLaTeX.com\" height=\"16\" width=\"41\" style=\"vertical-align: -4px;\"/>") |

# Discussion

## Some hot takes derived from the model

We make a note of some claims that are supported by the model. Since there is a large space of possible inputs we recommend the user specify their own input and not rely solely on our speculation.

### The community’s current spending rate is too low

Supposing the community indefinitely spends 2% of its capital each year on research and 2% on influence, the optimal spending schedule is around 30% better in the medium timelines, medium difficulty world.

### The optimal spending schedule is generally 5 to 15% better than the *default strategy*

Note: The default strategy is where you spend exactly the amount your money appreciates, and so your money remains constant. The greatest difference in utility comes from cases where it is optimal to spend lots of money now, for example in the (2030 median, hard difficulty) world, the optimal spending schedule is 15% better than the default strategy.

### In most cases, we should not ‘wager’ on long AGI timelines when we believe AGI timelines are short

A wager is, e.g., thinking that *‘although I think AGI is more likely than not in the next t years, it is intractable to increase the probability of success in the next t years and so I should work on interventions that increase the probability of success in worlds where AGI arrives at some time ![t'>t'](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/370e4205aba9c8298efb49ac2d5f0918.png "Rendered by QuickLaTeX.com")*. Saving money now, even though AGI is expected sometime soon, is only occasionally recommended by the model. One case occurs with (1) a sufficiently low probability of success but steep gains to this probability after some amount of preparedness that is achievable in the next few decades, (2) a low discount rate, and either (a) that influence does not get too much more expensive over time or (b) influence is not too important.

|  |
| --- |
|  |
| A ‘wager’ on long timelines in a case where we have 2030 AGI timelines. This case has a discount rate d=0.5%, the difficulty is hard[79](#easy-footnote-bottom-79-8199 "Probability of success if AGI is this year is 0.1%, and steepness <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-f3651552064b9a63ee3278254a268520_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#108;&#61;&#48;&#46;&#49;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"51\" style=\"vertical-align: 0px;\"/>") and the substitutability of research and influence is high[80](#easy-footnote-bottom-80-8199 "<img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-6c98d42cd6272be5516064c07bc2d0f7_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#114;&#104;&#111;&#32;&#61;&#48;&#46;&#56;\" title=\"Rendered by QuickLaTeX.com\" height=\"16\" width=\"56\" style=\"vertical-align: -4px;\"/>"). |

To some extent, there is a ‘sweet spot’ on the s-shaped success curve where we wager on long timelines. If we are able to push the probability of success to a region where the slope of the s-curve is large, we should spend a high rate until we reach this point. If we are stuck on the flatter far left tail such that we remain in that region regardless of any spending we do this century to stay in that area, we should spend at a more steady rate.

**In some cases, we should ‘wager’ on shorter timelines by spending at a high rate now**

This trivially occurs, for example, if you have a very high discount rate. A more interesting case occurs when (1) influence is poorly substituted by research[81](#easy-footnote-bottom-81-8199 "This is <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-acdcb3ab7c66c6fb178814c3cf9681a5_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#114;&#104;&#111;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"9\" style=\"vertical-align: -4px;\"/> is low, perhaps less than or equal to zero.") and either (a) influence depreciates quickly or (b) influence quickly becomes expensive.

|  |
| --- |
|  |
| A ‘wager’ on short timelines in a case where we have the 2050 AGI timeline. This case has ‘medium’ difficulty and low substitutability of research and influence[82](#easy-footnote-bottom-82-8199 "We take <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-7f311cc0c671d6295040ee068c01d916_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#114;&#104;&#111;&#32;&#92;&#97;&#112;&#112;&#114;&#111;&#120;&#32;&#48;\" title=\"Rendered by QuickLaTeX.com\" height=\"16\" width=\"42\" style=\"vertical-align: -4px;\"/>, so this is the Cobb-Douglas production function"). |

Since the opportunity to wager on short timelines only is available now, we believe more effort should go into investigating the wager.

## Limitations

We discuss the primary limitations here, and reserve some for the appendix. For each limitation, we briefly discuss how a solution would potentially change the results.

### Research is endogenous

The model does not explicitly account for research produced exogenously (i.e., not as a result of our spending). For example, it is plausible that research produced in academia should be included in our preparedness.

Exogenous research can be (poorly) approximated in the current model in a few different ways.

First, one could suppose that research appreciates over time and set ![\lambda_R>0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d2dea134ef827829827ae9184c92d063.png "Rendered by QuickLaTeX.com"). This supposes that research being done by outsiders is (directly) proportional to the research ‘we’ already have (where in this case, research done by outsiders is included in ![R(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/49a143387f6b63ffcf96d8841275fa6b.png "Rendered by QuickLaTeX.com")). Since we model exponential appreciation, appreciation leads to a research explosion. One could slow this research explosion by supposing the appreciation term was ![R(t)= \cdots \lambda_R R(t)^{\beta_R}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/9e7a352a57aaf34d275a6297c8765a59.png "Rendered by QuickLaTeX.com") for some ![0<\beta_R<1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/45a910af354a4cba40f04ce0f4ef18ef.png "Rendered by QuickLaTeX.com").

Second, one could suppose that exogenous research sometimes solves the problem for us, making our own research redundant. This can be approximated by increasing the discount rate to account for the ‘risk’ that our own work is not useful. This is unrealistic in the sense that we are ‘surprised’ by some other group solving the problem.

A possible modification to the model would be to add a term ![y_R(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e0c8c8be50d43f8b524c1600851902c2.png "Rendered by QuickLaTeX.com") to the expression for ![\dot{R}(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b831586106468bc76072ca0bf14ca4dd.png "Rendered by QuickLaTeX.com") that accounts for the exogenous rate of growth of research. Alternatively, one could consider a radically different model of research that considered our spending on research as simply speeding up the progress that will otherwise happen (conditioning on no global catastrophe).

We expect this is the biggest weakness of the model, especially for those with long AGI timelines. To a first approximation, if there is little exogenous research we do not need to account for it, and if there is a lot then our own spending schedule does not matter. Perhaps we might think our actions can lead us to be in either regime and our challenge is to push the world towards the latter.

### AGI timelines are independent of our spending schedule

We may hope that some real-world interventions may delay the arrival of AGI, for example, passing policies to slow AI capabilities work. The model does not explicitly account for this feature of the world at all.

One extension to the model would be to change the length of the fire alarm period to be a function of the amount of influence we have. We expect this extension to imply an increase in the relative spending rate on influence. Another, more difficult extension would be to consider timelines as function ![p(t, I(t))](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/3bd30ad86c5dd25d999f8c737539628f.png "Rendered by QuickLaTeX.com")  such that we can ‘push’ timelines down the road with more influence.

We expect that our ability to delay the arrival of AGI, particularly for shorter arrivals, is sufficiently minimal such that it would not significantly change the result. For longer timelines, this seems less likely to be the case.

### Research and capabilities are independent.

AI capabilities and our research influence each other in the real world. For example, AI capabilities may speed up research with AI assistants. On the other hand, spending large amounts on AI interventions may draw attention to the problem and speed up AI capabilities investment.

We allow for a depreciation of research, which can be used to model research becoming outdated as capabilities advance. One can also research becoming cheaper over time[83](#easy-footnote-bottom-83-8199 "Similar to how <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-00e84b3a6c4bed2f645baf247fc07077_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#99;&#40;&#116;&#41;\" title=\"Rendered by QuickLaTeX.com\" height=\"19\" width=\"27\" style=\"vertical-align: -5px;\"/> makes influence more expensive over time.") to account for capabilities speeding up our research.

On balance, we expect this limitation to not have a large effect. If one expects a ‘slow AI takeoff’ with the opportunity to use highly capable AI tools, one can use the fire alarm feature and set the returns to research during this period to be high.

### Diminishing returns, and other features, are constant

We model the returns to spending constant across time. However, actual funders seem to be bottlenecked by vetting capacity and a lack of scalable and high-return projects and so the returns to spending are likely to be high at the moment. Grantmakers can ‘seed’ projects and increase capacity such that it seems plausible that diminishing returns to spending will decrease in the future.

However, the model input only allows for constant diminishing marginal returns.

The model could be easily extended to use a function ![\eta_R(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/3048e4064c48a3931698d2d8d0763218.png "Rendered by QuickLaTeX.com") such that marginal returns to spending on research and influence changed over time, similar to how the real interest rate ![r(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/1cf8825a7a726a6ee93c73d15e987e67.png "Rendered by QuickLaTeX.com") changes over time. This would require more input from the user. Another extension could allow for the returns to be a function of how much was spent last year. However, such an extension would increase the model's complexity and decrease its usability, simplicity and (potentially) solvability.

This limitation also applies to other features of the model, such as the values ![\alpha_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2550f17b97b2268eebea86254d5c25d3.png "Rendered by QuickLaTeX.com") and ![\alpha_I](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/393f5533327000d88b0fe57871186b40.png "Rendered by QuickLaTeX.com").

### The optimal spending schedule is not always found

Most existing applications of optimal control theory to effective altruism-relevant decision-making have used systems of differential equations that are analytically solvable and have guarantees of optimality. Our model has neither property and so we must rely on optimization methods that do not always lead to a global maximum.

# Appendix

## Further limitations

### Many inputs are required from the user

There are around 40 free parameters that the user can set.

Many model features can be turned off. To turn off the following features:

* Variable interest rates, set ![r_{current}=r_{eventual}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/fcb9a8f409f810eb9a852b95311d24bc.png "Rendered by QuickLaTeX.com") or set ![\delta=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5266e127ee278f44dbf34aee4f360e48.png "Rendered by QuickLaTeX.com")
* Discount rate, set ![d=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/479714e83c018931712b22d30150f485.png "Rendered by QuickLaTeX.com")
* Appreciation or depreciation, set ![\lambda_R, \, \lambda_I=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b067cc13cd2cba91c66f8b2749129d09.png "Rendered by QuickLaTeX.com")
* Change in price of research and influence, set ![\alpha_R, \, \alpha_I=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4efa619553051bdb9224ff63a35ef4a9.png "Rendered by QuickLaTeX.com")
* Competition that changes the price of influence, set all competition levels to be 1 in all years.
* Only one of research or influence being necessary, set ![\gamma=1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/37f703973d88d399800a571cea42eb3f.png "Rendered by QuickLaTeX.com") (for no influence) or ![\gamma=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/a2b837f90e343131cfabaf9bb9d0807f.png "Rendered by QuickLaTeX.com") (for no research) [in this case, ![\rho](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/755b4a0f35e8d342d0840e253eea4fc3.png "Rendered by QuickLaTeX.com") does not matter]
* Fire alarm, set the expected fraction of money spendable to 0.

One can set parameters such that the model is equivalent to like the following system

     ![\[\begin{array}{ccl} \dot{M}(t)&=&r\cdot M(t)-x(t)\\[0.2cm] \dot{R}(t)&=&x_R(t)^{\eta_R} \\[0.2cm] U &=& \displaystyle\int_0^\infty p(t) \cdot \dfrac{1}{1+e^{-l(R(t)- R_0)}} dt \end{array}\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/7a2fd41707e2d0032002ba1de438388e.png "Rendered by QuickLaTeX.com")

Some results from this system[84](#easy-footnote-bottom-84-8199 "We have <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-8239a9e55ec835e7ab3ed00db5fa8e03_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#114;&#61;&#48;&#46;&#49;&#48;&#44;&#32;&#92;&#44;&#32;&#92;&#101;&#116;&#97;&#95;&#82;&#32;&#61;&#32;&#48;&#46;&#51;&#44;&#32;&#92;&#44;&#32;&#32;&#77;&#95;&#48;&#32;&#61;&#32;&#52;&#48;&#48;&#48;\" title=\"Rendered by QuickLaTeX.com\" height=\"16\" width=\"236\" style=\"vertical-align: -4px;\"/>"):

|  |  |  |
| --- | --- | --- |
|  |  |  |
|  |  |  |
|  |  |  |

### Appreciation of money is continuous and endogenous

The current growth rate of our money is continuous. However, this poorly captures the case where most growth is driven by the arrival of new donors with lots of capital. Further, any growth is endogenous - it is always in proportion to our current capital ![M(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d171c4e0139bb54367cca501366db62a.png "Rendered by QuickLaTeX.com").

One modification would be to the model arrival time of future funders by a stochastic process, for example following a Poisson distribution. For example, take

     ![\[\dot{M}(t)=r(t)\cdot M(t) - x_R(t) - x_I(t)  + \Phi(t),\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/6a9292c7aaba8b2fa988cf51d43ec8d6.png "Rendered by QuickLaTeX.com")

Where ![\Phi(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/a686605bd0bedf648d02e549b0a7f98a.png "Rendered by QuickLaTeX.com") can model endogenous and non-continuous growth of funding.

Following some preliminary experiments with a deterministic flux of funders, we are skeptical that this would substantially change the recommendations of the current model.

### The model only maximises the probability of ‘success’ (with constraints given by keeping money and spending non-negative)

We see two potential problems with this approach.

First, one may care about spending money on things other than making AGI go well. The model does not tell you how to trade-off these outcomes. The model best fits into a portfolio approach of doing good, such as Open Philanthropy’s [Worldview Diversification](https://www.openphilanthropy.org/research/worldview-diversification/). Alternatively, one may attach some value to having money leftover post-AGI.

Second, there may be outcomes of intermediate utility between AGI being successful and not. A simple extension could consider some function of the probability of success. A more complex extension could consider the utility of AGI conditioned on its arrival time and our preparedness that accounts for [near-miss scenarios](https://arbital.com/p/hyperexistential_separation/).

## Technical description

The funders have a stock of capital ![M(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d171c4e0139bb54367cca501366db62a.png "Rendered by QuickLaTeX.com"). This goes up in proportion to real interest at time ![t,\, r(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d8cb8d986ae96e0ed9113ede3f44c17c.png "Rendered by QuickLaTeX.com"), and down with spending on research, ![x_R(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dfab7abd1f5eb10d2f89d8c6ff91203.png "Rendered by QuickLaTeX.com"), and spending on influence, ![x_I(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/8ad805f47cc4585ea31ae2046c9e8b7a.png "Rendered by QuickLaTeX.com").

     ![\[\dot{M}(t) = r(t)\cdot M(t) - x_R(t) -x_I(t)\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/414d73fe004070d6d99f33d6a0530c85.png "Rendered by QuickLaTeX.com")

The funders have a stock of research which goes up with spending on research and can depreciate over time.

     ![\[\dot{R}(t) = x_R(t)^{\eta_R}\cdot R(t)^{\alpha_R}+\lambda_R R(t)\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/bb4d2e31870e59b2aa0c5b37cacbb48a.png "Rendered by QuickLaTeX.com")

Where

* ![\eta_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4cded6d2977150ae7a123c4bdc23af81.png "Rendered by QuickLaTeX.com") is the marginal returns to spending on research
* ![\alpha_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2550f17b97b2268eebea86254d5c25d3.png "Rendered by QuickLaTeX.com") is the increase or decrease in efficiency of spending due to the existing stock of research
* ![\lambda_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/49388f8c255514159c890f9b6e70f11f.png "Rendered by QuickLaTeX.com") is the rate of appreciation of the stock of research

Similarly, funders have a stock of influence ![I(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/32cf4c565a9bacb06e53e2369bc584b7.png "Rendered by QuickLaTeX.com") which obeys

     ![\[\dot{I}(t) = x_I(t)^{\eta_I}\cdot I(t)^{\alpha_I} c(t)-\lambda_I I(t)\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/82fc6856d4d547d6bf9818bd332794cd.png "Rendered by QuickLaTeX.com")

With constants mutatis mutandis from the research stock case and ![c(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5016c6770e3f9e0f3519394086c4699a.png "Rendered by QuickLaTeX.com") describes how the influence gained per unit money changes over time due to competition effects. That is, over time as the field of AGI influencers crowd each unit of influence can be more expensive.

### Fire alarm

We allow for the existence of an AGI fire alarm which tells us that AGI is exactly ![T_{FA}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/6f3cab46a37df29f9733e8216fcd7e96.png "Rendered by QuickLaTeX.com") years away and that we can spend fraction ![f](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2c39f42ff67efba6b5d5a7bf59b3a021.png "Rendered by QuickLaTeX.com") of our money on research and influence.

We write ![\hat{R}(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/a01fa96fcf5937b64e7aa626022063cc.png "Rendered by QuickLaTeX.com") and ![\hat{I}(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/8c87f3cbf78760d8b7d10201d3de4ed5.png "Rendered by QuickLaTeX.com") for the amount of research and influence we have in expectation at AGI take-off if the fire alarm occurred at time ![t](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dc427e6c482693df2e8d7ba9edecf38.png "Rendered by QuickLaTeX.com"). Within the fire alarm period, we suppose that

* we spend constant amounts on research and influence
* There is no appreciation or depreciation
* We have ![\eta_{I,FA}, \, \eta_{R,FA}, \, \alpha_{I,FA}, \alpha_{R, FA}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b71fbe9fbd593cda7dfab6cdbcb24d7f.png "Rendered by QuickLaTeX.com") which can be different from their pre-fire alarm values.

The first and second assumptions allow for analytical expression for ![\hat{R}(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/a01fa96fcf5937b64e7aa626022063cc.png "Rendered by QuickLaTeX.com") as a function of ![R(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/49a143387f6b63ffcf96d8841275fa6b.png "Rendered by QuickLaTeX.com") and ![M(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d171c4e0139bb54367cca501366db62a.png "Rendered by QuickLaTeX.com").

We write ![y_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/56df1147d53b8a442edc336192a73c0d.png "Rendered by QuickLaTeX.com") for the constant spending rate on research post-fire alarm. We take ![y_R=\dfrac{M(t)\cdot f}{T_{FA}}\cdot f_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2e58d37bfa1a21125c1a76e70d12ed75.png "Rendered by QuickLaTeX.com") where ![f_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d63d7bf54a3c9637e5f7013e8830f450.png "Rendered by QuickLaTeX.com") is the fraction of post fire-alarm spending. The system

     ![\[\tilde{R'}(\tau) =y_R^{\eta_{R, FA}}\cdot \tilde{R}(\tau)^{\alpha_{R, FA}} ,\, \tilde{R}(0) = R(t)\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/6d013c5db8cf0fb46fafafd57c3538c0.png "Rendered by QuickLaTeX.com")

has an [analytical solution](https://www.wolframalpha.com/input?i=dy%2Fdx+%3D+by%5Ea%2C+y%280%29%3Dd) and we take ![\tilde{R}(t) =\tilde{R}(T_{FA})](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/bd6b8739e6ae7a094ee038c2a5b9b3f5.png "Rendered by QuickLaTeX.com")

Similarly for research we take ![y_I = \dfrac{M(t)\cdot f}{T_{FA}}\cdot (1-f_R)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e9e322a1a0f8b5727b7fdc495d3405c7.png "Rendered by QuickLaTeX.com") and system

     ![\[\tilde{I}(\tau) = y_I^{\eta_{I,FA}}\cdot \tilde{I}(\tau)^{\alpha_{I,FA}}\cdot \tilde{c}(t), \, \tilde{I}(0) = I(t)\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/a534697848eefa36b8a27a8b83844734.png "Rendered by QuickLaTeX.com")

Where ![\tilde{c}(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2c6b2b621dcefa7ba78a1ce0ec81db14.png "Rendered by QuickLaTeX.com") is the competition factor at the start of the fire alarm period and is chosen by the user to either be a constant or function of ![c(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5016c6770e3f9e0f3519394086c4699a.png "Rendered by QuickLaTeX.com"). Note that ![\tilde{c}(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2c6b2b621dcefa7ba78a1ce0ec81db14.png "Rendered by QuickLaTeX.com") is a constant in the differential equation, so the system has an analytical solution of the research system above. Again we take ![\hat{I}(t) = \tilde{I}(T_{FA})](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/06bf351a88e0fd2d287fd684a660d1a2.png "Rendered by QuickLaTeX.com"). Note that the user can state that no fire alarm occurs; setting the ![f=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/322035cb9ca4d1ed9fcdcbee39d099a1.png "Rendered by QuickLaTeX.com") implies ![y_R=y_I=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e4d6e031a0d0249db71fe086b77831fb.png "Rendered by QuickLaTeX.com") and so ![\tilde{I'}(\tau) = \tilde{R'}(\tau) = 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2816bf101211b72e5919702f617ed15d.png "Rendered by QuickLaTeX.com") and so ![\hat{R}(t) = R(t), \hat{I}(t) = I(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/f14db67ea3b9f03fc18152458b81abed.png "Rendered by QuickLaTeX.com").

### Preparedness and success

Our preparedness ![S(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5feee354fdd40227a8f3d8bc37bde585.png "Rendered by QuickLaTeX.com") is given by

     ![\[S(t) :=(\gamma \cdot\hat{R}(t)^{\rho}+(1-\gamma)\cdot \hat{I}(t)^{\rho})^{1/\rho}\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d8e6e243097f51da543167775efca8ec.png "Rendered by QuickLaTeX.com")

Preparedness is the [constant elasticity of the substitution production function](https://en.wikipedia.org/wiki/Constant_elasticity_of_substitution) of ![\hat{R}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/3c338061c757364fbbfbe013fbe99ea0.png "Rendered by QuickLaTeX.com") and ![\hat{I}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/dc4fde5b639f561e877b115e483da1b9.png "Rendered by QuickLaTeX.com") where the user chooses ![\gamma](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/dd6823af35cc1bee47eb056352004b63.png "Rendered by QuickLaTeX.com") and ![\rho](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/755b4a0f35e8d342d0840e253eea4fc3.png "Rendered by QuickLaTeX.com").

Conditioning on AGI happening at time ![t](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dc427e6c482693df2e8d7ba9edecf38.png "Rendered by QuickLaTeX.com"), we take the probability of AGI being safe as

     ![\[Q(t) := 1+e^{-l\cdot(S-S_0)}\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b5e55b20d74e5bf6d1ac97122d96a882.png "Rendered by QuickLaTeX.com")

This is a [logistic function](https://en.wikipedia.org/wiki/Logistic_function) with constants ![l>0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/1074ef44c569a13a05eb08f663502d5c.png "Rendered by QuickLaTeX.com") and ![S_0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4ddbb4277ac8f367a5753622811bc646.png "Rendered by QuickLaTeX.com") determined by the user’s beliefs about the difficulty of making AGI safe.

Our objective is to maximize the probability that AGI is safe. We have an objective function

     ![\[U = \int_0^{\infty}Q(t)\cdot  p(t)\cdot e^{-dt} dt\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/842e9fa71e50a33998d82b8bff1dd613.png "Rendered by QuickLaTeX.com")

Where ![p(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e047cb96b673a8d692da97b97f78cede.png "Rendered by QuickLaTeX.com") is the user’s AGI timelines and ![d](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5f71587bd741524e4b4270aa128580aa.png "Rendered by QuickLaTeX.com") is some discount rate.

We have initial conditions ![M(0)=M_{0}, \; R(0)=R_{0}, \; \, I(0)=I_0.](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/c106d29102d6587966a28c9789c47b20.png "Rendered by QuickLaTeX.com")

### Solving the model

We apply standard optimal control theory results.

We have [Hamiltonian](https://en.wikipedia.org/wiki/Hamiltonian_(control_theory))

     ![\[H(t)=Q(t)\cdot p(t)\cdot e^{-dt}+v_M(t)\cdot \dot{M}(t)+v_R(t)\cdot \dot{R}(t)+v_I(t)\cdot \dot{I}(t)\]](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b1bb19d6dea04ac93e6aa2d357c3a3d7.png "Rendered by QuickLaTeX.com")

Where ![v_M(t), v_R(t), v_I(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/91df651eee7cdc440874e36e68b3c1b7.png "Rendered by QuickLaTeX.com") are the costate variables.

The optimal spending schedule, if it exists, necessarily follows

1. ![\dfrac{dH}{dx_R}=\dfrac{dH}{dx_I}=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/cba56b74c15cad3ed6519d4110c139b1.png "Rendered by QuickLaTeX.com")
2. ![v_M'(t) = \dfrac{dH}{dM}, \; v_R'(t) = \dfrac{dH}{dR}, \; v_I'(t)=\dfrac{dH}{dI}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/a213948c0b401b0bf3f0e9f73caeaff8.png "Rendered by QuickLaTeX.com")
3. ![M(T)=0, \; v_R(T)=0, \; v_I(T)=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/ac68ff63aeeb6b54582f1b6606d89681.png "Rendered by QuickLaTeX.com")

We solve this [boundary value problem](https://en.wikipedia.org/wiki/Boundary_value_problem) using SciPy’s *solve\_bvp* function and apply further optimisation methods to avoid local optima.

## Model guide

The model is a Python Notebook accessible on Google Colaboratory [here](https://colab.research.google.com/drive/17f0yTYcFSBihZFd8_N7yRjF2XYJDjvBZ?usp=sharing).

Any cells that contain “**User guide**” are for assisting with the running of the notebook.

Below the initial instructions, you will find the user input parameters.

In the next section of this document we describe the parameters in detail and our own guesses.

## Explaining and estimating the model parameters

We discuss the parameters in the same order as in the notebook.

*Note, the estimates given are from Tristan and not necessarily endorsed by Guillaume.*

*Epistemic status: I’ve spent at least five minutes thinking about each, sometimes no more.*

### AI timelines

We elicit user timelines using two points on the [cumulative distribution function](https://en.wikipedia.org/wiki/Cumulative_distribution_function) and fit a [log-normal distribution](https://en.wikipedia.org/wiki/Log-normal_distribution) to them.

We note Metaculus’ [*Date of Artificial General Intelligence* community prediction](https://www.metaculus.com/questions/5121/date-of-artificial-general-intelligence/): as of 2022-10-06, lower 25% 2030, median 2040 and upper 75% 2072.

Note that since our log-normal distribution is parameterised by two pairs of (year, probability by year), the three distinct Metaculus interquartile pairings will give different distributions.

### Discount rate

The discount rate needs to factor in both non-AGI existential risks as well as catastrophic (but non-existential) risks that preclude our AI work from being useful or any unknown unknowns that have some per year risk.

We choose ![d=2\%,](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2a3ab49aafa1a72d241eb74171ad633e.png "Rendered by QuickLaTeX.com") implying an AGI success in 2100 is worth ![e^{-\frac{2}{100}\cdot 78} = 21\%](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/672e6bdf11ee46ef42e342e0d3757f6f.png "Rendered by QuickLaTeX.com") as much as a win today. As we discuss in the limitations section, the discount rate ![d](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5f71587bd741524e4b4270aa128580aa.png "Rendered by QuickLaTeX.com") can also account for *other* people making AGI successful, though this interpretation of ![d](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5f71587bd741524e4b4270aa128580aa.png "Rendered by QuickLaTeX.com") is not unproblematic.

Of relevance may be:

* The [Metaculus forecast on World War Three before 2050](https://www.metaculus.com/questions/2534/world-war-three-before-2050/), current median 21%.
* The [Metaculus forecast on Human Extinction by 2100](https://www.metaculus.com/questions/578/human-extinction-by-2100/), current median 3%
* The Metaculus notebook from Tamay which synthesis Metaculus forecasts to come to median 18% of global catastrophe this century.

Our 90% confidence interval for ![d](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5f71587bd741524e4b4270aa128580aa.png "Rendered by QuickLaTeX.com") is ![0.5\% < d < 5\%](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/c956fab541eadb8346726e47078e4528.png "Rendered by QuickLaTeX.com")

### Money

#### Starting money

As of 2022-10-06, Forbes estimates [Dustin Moskovitz](https://www.forbes.com/profile/dustin-moskovitz/?sh=4417b291dd34) and [Sam Bankman Fried](https://www.forbes.com/profile/sam-bankman-fried/?sh=1d71a92c4449) have wealth of $8,200m and $17,000m respectively. [Todd (2021)](https://80000hours.org/2021/07/effective-altruism-growing/) estimates $7,100m from other sources in 2021 giving a total of $32,300m within the effective altruism community.

How much of this is committed to AI safety interventions?

Open Philanthropy [has spent $157m on AI-related interventions](https://effectivealtruismdata.com/#op-grants-categories), of approximately $1500m spent so far. Supposing that roughly 15% of all funding is committed to AGI risk interventions gives at least $4,000m.

Our 90% confidence interval is ![$1,000 m < M_0 < \15,000 m](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/85ebf7d6fa3b427493bfbbcd537ed2ac.png "Rendered by QuickLaTeX.com").

#### Real interest rate

We suppose that we are currently at some interest rate rcurrent which decreases over time (at rate ) to ![r_{eventual}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/99215a229c6b20ff40a8394ef6a203d0.png "Rendered by QuickLaTeX.com").

Supposing the movement had $10,000m in 2015 and $32,300 in mid-2022, money in the effective altruism community has grown 21% per year.

We take ![r_{current}=20\%](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2907950b67160122bfab653c81d6a531.png "Rendered by QuickLaTeX.com").  Our 90% confidence interval is ![5\% < r_{current} < 40\%](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/11523f65b433dd8ce5dac5662769552f.png "Rendered by QuickLaTeX.com").

[Historical S&P returns are around 8.5%](https://www.investopedia.com/ask/answers/042415/what-average-annual-return-sp-500.asp#:~:text=Adjusted%20for%20inflation%2C%20the%20historical,return%20is%20only%20around%208.5%25.). There are reasons to think the long-term rate may be higher - such as increase in growth due to AI capabilities -  or lower  - there is a selection bias in choosing a successful index. We take ![r_{eventual}=8,5\%](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/89e4f51d7b2d8537eddfe139073c5147.png "Rendered by QuickLaTeX.com"). Our 90% confidence interval is ![3\% < r_{current}< 15\%](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/cb7ac6da4cafa34e02f04dcf8835672e.png "Rendered by QuickLaTeX.com").

![\delta](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/0053c59586f7c0c528abc435daa86e67.png "Rendered by QuickLaTeX.com") is the rate at which the real interest rate moves from ![r_{current}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5465e01544bab7398c56755cd9473e08.png "Rendered by QuickLaTeX.com") to ![r_{eventual}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/99215a229c6b20ff40a8394ef6a203d0.png "Rendered by QuickLaTeX.com"). The effective altruism and AI safety movement has been growing substantially for the last 10 to 15 years. Naively, suppose that we’re in the middle of the growth period. We take = 0.2, which implies that capital will only be growing 1.15 times ![r_{eventual}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/99215a229c6b20ff40a8394ef6a203d0.png "Rendered by QuickLaTeX.com") ten years from now.

Our 90% confidence interval is ![0.02 <\delta<1.5](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/cc0e346ab14cda803084f7d72aa051f1.png "Rendered by QuickLaTeX.com").

### Research and influence

#### Marginal returns to spending

***Influence***

The constant ![\eta_I](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/3e1a936abfb19a6b8b8d26983545acc7.png "Rendered by QuickLaTeX.com") controls the marginal returns to spending on influence. For ![\eta_R < 1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/7f324442d1442eb93849f595bea9fe93.png "Rendered by QuickLaTeX.com") we receive *diminishing* marginal returns.

The top ![x](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5e5f0dd3e7df9b09fcd87a0fbe7bec7c.png "Rendered by QuickLaTeX.com")  fraction of spending per year on influence leads to ![x^{\eta_I}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/6f7b3832d01d264d782b9a4713557c10.png "Rendered by QuickLaTeX.com") fraction of increase in growth of influence in that year. For example, ![\eta_I=0.15](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/066c1d9ffbcb1c2d84f32c21ee3a77cb.png "Rendered by QuickLaTeX.com") implies the top 20% of spending leads to roughly 80% of returns i.e. the [Pareto principle](https://en.wikipedia.org/wiki/Pareto_principle).

We note that influence spending can span many orders of magnitude and this suggests reason to think there are high diminishing returns (i.e. low ![\eta_I](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/3e1a936abfb19a6b8b8d26983545acc7.png "Rendered by QuickLaTeX.com")). For example, one community builder may cost on the order of ![$10^5](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/86b4b1fe697a1db8a391f8c5176ba26a.png "Rendered by QuickLaTeX.com") per year, but investing in AI labs with the purpose of influencing their decisions may cost on the order of ![$10^8](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/decb9e722f662c1ce1f000957d3e819d.png "Rendered by QuickLaTeX.com") per year.

We take ![\eta_I=0.2,](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b0fb2206e71f06cc53a7ba29e0ac47d9.png "Rendered by QuickLaTeX.com") which implies doubling spending on influence lead to ![2^{0.2}=1.15](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/674185b36976de9a8ce8cb17643b605c.png "Rendered by QuickLaTeX.com") times more growth of influence Our 90% confidence interval is ![0.1 < \eta_I < 0.5](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/f32f34492ca1f2b035c4a7503681e368.png "Rendered by QuickLaTeX.com").

***Research***

The constant ![\eta_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4cded6d2977150ae7a123c4bdc23af81.png "Rendered by QuickLaTeX.com") acts in the same way for research as ![\eta_I](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/3e1a936abfb19a6b8b8d26983545acc7.png "Rendered by QuickLaTeX.com") does for influence.  
We take ![\eta_R=0.3](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/68af4fc5917156c50b99c19979ae4a01.png "Rendered by QuickLaTeX.com"), which implies a doubling of research spending leads to ![2^{0.3}=1.23](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5a6aea8e1998e69b8707308bb8f50240.png "Rendered by QuickLaTeX.com") times increase in research growth and that 20% of the spending in research accounts for ![(20\%)^{0.3}=60\%](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/713dc161f610c9ffbd3409f89d539458.png "Rendered by QuickLaTeX.com") of the increase in research growth.

Potential sources for estimating ![R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/99b386a6e31a7d4ed3f1ceca88aca033.png "Rendered by QuickLaTeX.com") include using the distribution of karma on the Alignment Forum, citations in journals or estimates of researchers’ outputs.

Our 90% confidence interval is ![0.1 < \eta_R < 0.6](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/82ba40512772cd4739497b8bb79dd9ad.png "Rendered by QuickLaTeX.com").

#### Change in price of the stocks when you have more

***Influence***

![\alpha_I](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/393f5533327000d88b0fe57871186b40.png "Rendered by QuickLaTeX.com") controls how the price of influence changes as the amount of influence we have changes.

![\alpha_I > 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d38e7ff712f87d64acb9c16ffefbf4bc.png "Rendered by QuickLaTeX.com") implies that influence becomes cheaper as we get more influence. Factors that push in this direction include:

* The existence of  network effects related to being trusted and having a good reputation, For example,
  + It may become easier to convince other people to trust us
  + We may be given access to exclusive opportunities.
* [The ‘clear wins’ model of political capital](https://www.lesswrong.com/posts/vavnqwYbc8jMu3dTY/ai-coordination-needs-clear-wins)

![\alpha_I < 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/154e8dd894e8a19e6daf6b97eecebdfb.png "Rendered by QuickLaTeX.com") implies that influence becomes more expensive as we get more influence. Factors that point in this direction include:

* We can run out of opportunities to gain influence or only difficult opportunities remain.
* We could be seen as suspicious for amassing power, and trust in us decreases.

For ![\alpha_I=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d5f726a6dd77394d60dc4541274d896c.png "Rendered by QuickLaTeX.com") the price is constant.

On balance, we think the former reasons outweigh the latter, and so take ![\alpha_I=0.3](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/cf4d76b3bd20f518d35fbfa593764e8b.png "Rendered by QuickLaTeX.com"). This implies a doubling of influence leads to one unit of spending on influence leading to ![2^{0.3}=1.23](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5a6aea8e1998e69b8707308bb8f50240.png "Rendered by QuickLaTeX.com") times more growth in influence compared to one unit of spending without this doubling. Our 90% confidence interval is ![-0.75 < \alpha_I < 1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2352de11e82c89c80e07124d8fafb2a0.png "Rendered by QuickLaTeX.com").

***Research***

The constant ![\alpha_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2550f17b97b2268eebea86254d5c25d3.png "Rendered by QuickLaTeX.com")  acts in the same way for research as αI does for influence.

![\alpha_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2550f17b97b2268eebea86254d5c25d3.png "Rendered by QuickLaTeX.com") controls how the price of influence changes as the amount of influence we have changes.

![\alpha_R > 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/ccfe4f3e0841282c1f0d1109219310d8.png "Rendered by QuickLaTeX.com") implies that research becomes cheaper as we get more research. Factors that push in this direction include:

* Research becoming more parallelizable. For example, sub-questions are found that can be worked on with less context or more standard backgrounds.
* Attracting greater talent to the field once you have developed the field.

![\alpha < 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/57c0d150c7c171efd9f3c5262842017d.png "Rendered by QuickLaTeX.com") implies that research becomes more expensive as we get more research. Factors that push in this direction include:

* Research becoming more serial. That is, the field is increasingly bottlenecked by progress in a few key areas.
* The costs of getting up to speed with research increase as we accumulate new research. For example, new researchers need to learn increasingly more background material before being able to contribute.

We are uncertain about the net effect of the above contributions, and so take ![\alpha_R = 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/f69917df248094516a1335b2058db6cc.png "Rendered by QuickLaTeX.com"). Our 90% confidence interval is ![-1.5 < \alpha_R < 1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b773d4440102c9abaed5cac200251945.png "Rendered by QuickLaTeX.com").

#### Depreciation of stocks

***Influence***

![\lambda_I](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/0e6e54a79db296d91cfc6334ebab59d3.png "Rendered by QuickLaTeX.com") controls the rate of appreciation, for ![\lambda > 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/fc315b603c7c36b8758f5d03954d8564.png "Rendered by QuickLaTeX.com"), or depreciation, for ![\lambda < 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/815a1d87dbff3cac829bb00de624ff85.png "Rendered by QuickLaTeX.com"), of our stock of influence. It seems very likely that ![\alpha_I < 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/154e8dd894e8a19e6daf6b97eecebdfb.png "Rendered by QuickLaTeX.com") since

* AGI labs we have influence over can decrease in relative importance.
* The number of AGI labs and people working on AGI increases, and so our relative influence decreases

We take ![\lambda=-0.25](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/0eece4bffa714a7a260199826eafbd6c.png "Rendered by QuickLaTeX.com"), which implies a half-life of around  ![\dfrac{\log 50\%}{-0.25}=2.8](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b882a4de2bf8a3dfb846dd456fddfe5a.png "Rendered by QuickLaTeX.com")  years. Our 90% confidence interval is ![-3< \lambda_I < -0.15](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/c1a023e8dcae314f455a3cdf75166ded.png "Rendered by QuickLaTeX.com").

***Research***

![\lambda_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/49388f8c255514159c890f9b6e70f11f.png "Rendered by QuickLaTeX.com") controls the rate of appreciation, for ![\lambda_R>0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d2dea134ef827829827ae9184c92d063.png "Rendered by QuickLaTeX.com"), or depreciation, for ![R<0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/30585d078bc3c82c1ef466de7304eec5.png "Rendered by QuickLaTeX.com"), of our stock of influence.

We expect research to depreciate over time. Research can depreciate by

* Becoming less relevant over time
* Be lost, forgotten or otherwise inaccessible

One intuition pump is to ask *what fraction of research on current large language models will be useful if AGI does not come until 2050*? We guess on the order of 1% to 30%, implying - if all our research was on large language models - a value of ![\lambda_R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/49388f8c255514159c890f9b6e70f11f.png "Rendered by QuickLaTeX.com") between ![\dfrac{\log 1\%}{38}=-0.12](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/01a883b020a44b80a25b573a9f18618a.png "Rendered by QuickLaTeX.com") and ![\dfrac{\log 30\%}{38}=-0.12](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/f355d4ccbadf96727f192faf33a76d31.png "Rendered by QuickLaTeX.com"). Note that for ![\alpha_R >0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/8168d7e3009824b93683bb2c355bfc89.png "Rendered by QuickLaTeX.com"), such research can be instrumentally useful for later years due to its ability to make future work cheaper  by,  for example,  attracting new talent.

We take ![\lambda_R=-0-03](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/d8d783eac425c6ea25187a3e4df24ba5.png "Rendered by QuickLaTeX.com"). Our 90% confidence interval is ![-0.2<\lambda_R<-0.01](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/f93cefb9197ce64d204f8a7dad45944a.png "Rendered by QuickLaTeX.com").

### Competition effects

We allow for influence to become more expensive over time. The primary mechanism we can see is due to (a) competition with other groups that want to influence AI developers, and (b) competition within the field of AI capabilities, such that there are more organisations that could potentially develop AGI.

We suppose the *influence per unit spending*decreases over time following some S-shape curve, and ask for three points on this curve.

The first data point is the first year in which money was spent on influence. Since one can consider community building or spreading AI risk ideas (particularly among AI developers) as a form of  influence, the earliest year of spending is unclear.  We take 2015 ([the first year Open Philanthopy made grants in this area](https://en.wikipedia.org/wiki/Machine_Intelligence_Research_Institute#History)). The relative cost of influence is set to 1 in this year.

We then require to further years, as well as influence per unit spending relative to the the first year of spending.

Our best guess is  (2017, 0.9) - that is, in 2017 one received 90% as much influence per unit spending as one would have done in 2015-  and (2022, 0.6).

The final input is the minimum influence per unit spending that will be reached be take this to be 0.02. That is, influence will eventually be ![50x](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b20257da9c9def5dde8ac964e5b5de82.png "Rendered by QuickLaTeX.com") more expensive per unit that it was in 2015. Our 90% confidence interval is (0.001, 0.1).

### Historical spending on research and influence

The model uses this data to calculate the quantities of research and influence we have now. Rough estimates are sufficient.

The Singularity Institute (now MIRI) was founded in 2000 and switched to work on AI safety in 2005. We take 2005 as the first year of spending on research.

Open Philanthropy [has donated $243.5m](https://www.openphilanthropy.org/focus/potential-risks-advanced-ai/) to risks from AI since its first grant in the area in August 2015. We very [roughly categorised each grant by research : influence fraction,](https://docs.google.com/spreadsheets/d/1XpWNGyho_kkSkVlMsqnddrhnEYW7MRQBmLX0wITYxGQ/edit?usp=sharing) and estimate that $132m has been spent on research and $111m on influence. We suppose that Open Philanthropy has made up two-thirds of the overall spending, giving totals of $198m and $167m.

We guess that the research spending, which started in 2005, has been growing at 25% per year and influence spending has been growing 40% per year since starting in 2015.

### Fire alarm

By default, in the results we show, we assume *no*fire alarm in the model. This is achievable by settingthe expected fraction of money spendable to 0. When considering the existence of a fire alarm, we take the following values.

For the fire alarm duration we ask *Supposing that the leading AI lab has reached an AGI system that they are not deploying out of safety concerns, how far behind is a less safety-conscious lab?* We guess this period to be half a year.

Our 90% confidence interval for this period, if it exists, is (one month, two years).

One may think that expected fraction of money spendable during the fire alarm is less than 1 for reasons such as

* Not being certain that the AGI fire alarm has gone off [though we don’t model other false positives, and are only supposing that we may worry that this actual fire alarm is a false positive]
* Limited liquidity of the capital
* Bottlenecked by transaction speeds

We take 0.1 as the expected fraction of money spendable with 90% confidence interval  (0.01, 0.5).

#### Returns to spending during the fire alarm

During the fire alarm period, we enter a phase with no appreciation or depreciation of research or influence and a separate marginal returns to spending ![-\eta_{R,FA}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/aaa145e78034b267d5441b9c5ba47a14.png "Rendered by QuickLaTeX.com") and ![\eta_{I,FA} -](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/8108164025ddcf68dd86272bed073874.png "Rendered by QuickLaTeX.com") can apply.

Some reasons to think ![\eta_{FA} < \eta](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/f79fc9c0b1b75c5bb3bc0406f575c60c.png "Rendered by QuickLaTeX.com") (worse returns during the fire alarm period)

* There is general panic or uncertainty around what to do and worse coordination leading to wasted effort
* The most useful technical work can only be done within highly secure environments to avoid leaks to the competitor labs
* The labs that are reaching AGI become increasingly averse to being influenced from the outside, since there may be more bad actors targeting them.
* People may be less incentivised by money if they believe AGI is near.

Some reasons to think the ![\eta_{FA}>\eta](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/f4bbe8d6074904e871598b1ffef33ad6.png "Rendered by QuickLaTeX.com") (better returns during the fire alarm period)

* There are unique opportunities that arise during this period
* There is clarity over what AGI will look like.
* We can actually execute a plan that has been refined in the pre-fire-alarm period
* We can take riskier actions that would damage our reputation during the pre-fire alarm period.
* Some people will be more motivated to work harder
* Some people will be more open to the idea of AI safety, given that capabilities are at a high level

We expect that the returns to research spending will be very low, and take ![\eta_{R,FA}=0.05](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/c09b48c77d9bbc65823fd66725a92381.png "Rendered by QuickLaTeX.com"), implying that the amount of research we can do in the post-fire-alarm period is not very dependent on the money we have.

We expect that returns to influence spending will be less than in the period before, lower. We take ![\eta_{I,FA}=0.1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/20519ce72ee9263c2cfe7eda87653112.png "Rendered by QuickLaTeX.com").

#### Change in price of the stocks when you have more

In the fire alarm phase, the cost per unit of research and influence can also change depending on the amount we already have.

We expect ![\alpha_{I,FA}>\alpha_I](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/c49af71bdfbeca2367f504ac23fbb087.png "Rendered by QuickLaTeX.com") and ![\alpha_{R,FA}>0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/bad3436193f5a37cf1b4057b8e5dc648.png "Rendered by QuickLaTeX.com"). That is, during the fire alarm period it is even cheaper to get influence once you already have some than before this phase and that this effect is greater during the fire alarm period (the first inequality). In the case there is panic, it seems people will be looking for trustworthy organisations to defer to and execute a plan.

We expect ![\alpha_{R,FA}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/db9b54de0f6131711a667208af613c95.png "Rendered by QuickLaTeX.com") That is, during the fire alarm period the amount of existing research decreases the cost of new research.

During the fire alarm period, it seems likely that only a few highly skilled researchers - perhaps within the AI lab - will have access to the information and tools necessary to conduct further useful research. The research at this point is likely highly serial: the researchers trying to focus on the biggest problems. Existing research may allow these few researchers to build on existing work effectively.

We take both ![\alpha_{I,FA}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/eb9a874f456877f9a715d41e7decca10.png "Rendered by QuickLaTeX.com") and ![\alpha_{R,FA}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/db9b54de0f6131711a667208af613c95.png "Rendered by QuickLaTeX.com") to be 0.3, implying that a doubling of research *before*the fire-alarm period increases the stock output *during* the fire-alarm period by ![2^{0.3}=1.23](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5a6aea8e1998e69b8707308bb8f50240.png "Rendered by QuickLaTeX.com") times.

#### Competition during the fire alarm period

### Preparedness and probability of success

#### Preparedness

Preparedness at time ![t](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dc427e6c482693df2e8d7ba9edecf38.png "Rendered by QuickLaTeX.com") is [a function](https://en.wikipedia.org/wiki/Constant_elasticity_of_substitution) of the fire-alarm adjusted research and influence that takes two parameters, the share parameter  that controls the relative importance of research and influence and parameter , that controls the substitutability of research and influence.

![\gamma](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/dd6823af35cc1bee47eb056352004b63.png "Rendered by QuickLaTeX.com") is the *share parameter*. Increasing ![\gamma](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/dd6823af35cc1bee47eb056352004b63.png "Rendered by QuickLaTeX.com") increases the ratio {increase to preparedness when increasing research by 1 unit} to {increase to preparedness when increasing influence by 1 unit}.

![\gamma](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/dd6823af35cc1bee47eb056352004b63.png "Rendered by QuickLaTeX.com") cannot be derived from first principles due to our choice of units. Instead, we recommend running the cell and using the available statistics and graphs to inform your guesses. We take ![\gamma=0.6](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e09da5ca51937db4dc3411853cdf1576.png "Rendered by QuickLaTeX.com").

![\rho](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/755b4a0f35e8d342d0840e253eea4fc3.png "Rendered by QuickLaTeX.com") controls the subsitutability of research and influence. If you think it is possible to make AGI go well with lots of research and *zero* influence or zero research and lots of influence, then consider setting ![\rho=1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/47edccc9464d102e40ab0d658fdca865.png "Rendered by QuickLaTeX.com"). Otherwise, you should set ![\rho<1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/561804bb3e98d8488fa6514e1604cf39.png "Rendered by QuickLaTeX.com").

Decreasing ![\rho](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/755b4a0f35e8d342d0840e253eea4fc3.png "Rendered by QuickLaTeX.com") decreases the subsitutability of research and influence. In the limit as ![\rho\rightarrow -\infty](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b5890087a1ea0af5b7d5feebf1a15e13.png "Rendered by QuickLaTeX.com"), our preparedness can be entirely bottlenecked by the stock we have the least (weighted by ![\gamma](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/dd6823af35cc1bee47eb056352004b63.png "Rendered by QuickLaTeX.com")).

![\rho=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/ab69d70a59e628bee83ada11ce46d91a.png "Rendered by QuickLaTeX.com") gives the [Cobb-Douglas production function](https://en.wikipedia.org/wiki/Cobb%E2%80%93Douglas_production_function), though to avoid a case-by-case situation in the programming, you cannot set ![\rho=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/ab69d70a59e628bee83ada11ce46d91a.png "Rendered by QuickLaTeX.com") and instead can choose value close to ![0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/296b29a9de94ee6c00d2ed81833ea202.png "Rendered by QuickLaTeX.com").

Again, we recommend picking values and running the cell to see the graph. We choose ![\rho=0.3](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/70d52f100ec9bf4a50a66c311c6e7421.png "Rendered by QuickLaTeX.com"). We think that the problem is mainly a technical problem, but in practise cannot be solved without influencing AI developers.

#### Probability of success

The probability of success at time t conditioned on AGI’s arrival at time t is a function of our preparedness at that time. The function is an S-shaped [logistic](https://en.wikipedia.org/wiki/Logistic_function)[function](https://en.wikipedia.org/wiki/Logistic_function) and it is determined by two inputs.

The first input is the probability of success if AGI arrived this year. That is, given our existing stocks of research and influence - this input doesn't consider any fire alarm spending.  The second input determines the steepness of the S-shaped curve.

We take (10%, 0.15).

*A note on the probability of success*

Suppose you think we are in one the following three worlds

* World A: AGI will go certainly well, regardless of what we do
* World B: AGI might go well, and we can influence the probability it does
* World C: AGI will certainly not go well, regardless of what we do

Then, in the input you should imagine you should give your inputs as they are in your world B model. We keep the probability of success curve between 0 and 1, but one could linear transform it to be greater than the probability of success in the A world and less than the probability of success in the C world. Since the objective function is linear in the probability of success, such a transformation has no effect on the optimal spending schedule.

## Alternate model

In an alternate model, we suppose the funder has a stock of *things that grow ![K(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/eb7cdcd59eff9483d00dee07eb2f1b68.png "Rendered by QuickLaTeX.com")* which includes things such as skills, people, some types of knowledge and trust. They can choose to spend this stock ![K(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/eb7cdcd59eff9483d00dee07eb2f1b68.png "Rendered by QuickLaTeX.com") at some rate ![x(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b42f36b2ba2868f587110da7ebbfd708.png "Rendered by QuickLaTeX.com") to produce a stock of *things that depreciate* ![C(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/515955a3ad1ae2fa344a290c1aa9e110.png "Rendered by QuickLaTeX.com") that are immediately helpful in increasing the probability of success. This could comprise things such as the implementation of safety ideas on current systems or the product of asking for favours of AI developers or policymakers.

We say that spending capacity to create ![C(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/515955a3ad1ae2fa344a290c1aa9e110.png "Rendered by QuickLaTeX.com") is *crunching*and the periods with high ![x(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/b42f36b2ba2868f587110da7ebbfd708.png "Rendered by QuickLaTeX.com") are*crunch time.*

The probability we succeed at time ![t](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4dc427e6c482693df2e8d7ba9edecf38.png "Rendered by QuickLaTeX.com") is a function of ![\hat{C}(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e8ff5d3228c8d14aeec7986440b5a8e2.png "Rendered by QuickLaTeX.com") which is ![C(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/515955a3ad1ae2fa344a290c1aa9e110.png "Rendered by QuickLaTeX.com") plus any last-minute spending that occurs with a fire alarm. Specifically, it is another [S-shaped curve](https://en.wikipedia.org/wiki/Logistic_function).

![](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/51a7ae8fcb5ec8195a97ab1b88b6b816.png)

A diagram of the alternate model

### Formalisation

|  |  |
| --- | --- |
| Time evolution of things that grow | \dot{K}(t)=r(t)\cdot K(t)-x(t) |
| Time evolution of things that depreciate | \dot{C}(t)=x(t)^{\eta}\cdot c(t)-\lambda_C\cdot C(t) |
| Post-fire alarm total of things that depreciate | \hat{C}(t)=C(t)+\left(\dfrac{K(t)\cdot f}{T_{FA}}\right)\cdot T_{FA} |
| The probability of success given AGI at t | Q(t)=(1+e^{\kappa \cdot (\hat{C}(t)-\sigma)})^{-1} |
| Objective function | U=\int_0^{\infty} Q(t)\cdot p(t)\cdot e^{-dt}dt |

Recall that ![f](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2c39f42ff67efba6b5d5a7bf59b3a021.png "Rendered by QuickLaTeX.com") is the expected fraction of money spendable post-fire alarm and ![T_{FA}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/6f3cab46a37df29f9733e8216fcd7e96.png "Rendered by QuickLaTeX.com") is the expected duration of the fire alarm. The equation for ![\hat{C}(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e8ff5d3228c8d14aeec7986440b5a8e2.png "Rendered by QuickLaTeX.com") is thus simply the result of spending at rate ![\dfrac{K(t)\cdot f}{T_{FA}}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/15a62527b8dc6e01cb37a70f45b09e40.png "Rendered by QuickLaTeX.com") for duration ![T_{FA}](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/6f3cab46a37df29f9733e8216fcd7e96.png "Rendered by QuickLaTeX.com").

### Estimating parameters

The alternate model shares the following parameters and machinery with the research-influence model

* AGI timelines, ![p(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e047cb96b673a8d692da97b97f78cede.png "Rendered by QuickLaTeX.com")
* Discount rate, ![d](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5f71587bd741524e4b4270aa128580aa.png "Rendered by QuickLaTeX.com")
* Growth rate ![r(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/1cf8825a7a726a6ee93c73d15e987e67.png "Rendered by QuickLaTeX.com")
* Competition factor ![c(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5016c6770e3f9e0f3519394086c4699a.png "Rendered by QuickLaTeX.com")
* The duration of the fire alarm and expected fraction of money spendable

The new inputs include

* Diminishing returns to spending on direct work ![\eta](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/2fb5422a2f6cbe6ebc9e2dfdd7654b6c.png "Rendered by QuickLaTeX.com")
* Depreciation of the direct work ![\lambda_C](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/7a343f9e4285554ae11d0408f51c015f.png "Rendered by QuickLaTeX.com")
* Probability of success as a function of our direct work

#### Growth rate

![r(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/1cf8825a7a726a6ee93c73d15e987e67.png "Rendered by QuickLaTeX.com") now refers to the growth of the community's capacity,  of which money is one component. Things that grow include our prioritisation knowledge and general understanding of AI risk increases each year, skills of people in the movement and connections between people.

We expect the growth in capacity to decrease over time since some of our capacity is money and the same reasons will apply as in the former model. We suppose ![r_{current}=40\%, \; r_{eventual}=20\%](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/ddf720e22c5cb17b1c2ecd2cd2f17587.png "Rendered by QuickLaTeX.com"), and ![\delta=0.2](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/1a5224d0d06afa36ec7426e07e839dff.png "Rendered by QuickLaTeX.com").

#### Competition factor

The factor ![c(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5016c6770e3f9e0f3519394086c4699a.png "Rendered by QuickLaTeX.com"), which in the former model controlled how influence becomes more expensive over time, controls how the cost of doing direct work - producing ![C(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/515955a3ad1ae2fa344a290c1aa9e110.png "Rendered by QuickLaTeX.com") - becomes more expensive over time. . Only some spending to produce ![C(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/515955a3ad1ae2fa344a290c1aa9e110.png "Rendered by QuickLaTeX.com") is in competitive domains (such as influencing AI  developers) while some is non-competitive, such as implementing safety features in state-of-the-art systems.

We suppose that ![c(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5016c6770e3f9e0f3519394086c4699a.png "Rendered by QuickLaTeX.com") has a minimum 0.5 and otherwise has the same factors as in the former research-influence model.

#### Diminishing returns to spending

This controls the degree of diminishing returns to ‘crunching’. For reasons similar to those given for ![R](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/99b386a6e31a7d4ed3f1ceca88aca033.png "Rendered by QuickLaTeX.com") and ![I](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/cc93bcbeac0b9e6763f634a03b62f20e.png "Rendered by QuickLaTeX.com") in the main model, we take ![\eta=0.3](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/0328ec877e3ae0acb11c0feafdfbd151.png "Rendered by QuickLaTeX.com"). Our 90% confidence interval is ![0.1 < \eta < 0.6](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/43b3ee44a43d06660caa18dc1bcfed84.png "Rendered by QuickLaTeX.com").

#### Depreciation of the direct work

This controls how long our crunch time activities are useful for i.e. the speed of depreciation. We take ![\lambda_C=-0.5](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/cbbea43c32aecf6bcf71ff39947d643d.png "Rendered by QuickLaTeX.com") which implies that after one ![e^{-1}=37\%](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/86705cf1a75d7b87b1ee896f265309e5.png "Rendered by QuickLaTeX.com")  of the direct work is still useful.

#### Probability of success

To derive the constants used in the S-shaped curve, we ask for the probability of success after some hypothetical where we've spent some fraction of our capacity for one year.

Our guess is that after spending half of our resources this year, we’d have a 25% chance of alignment success *if*AGI arrived this year. Note that this input does not account for any post-fire-alarm spending.

### Results

Unsurprisingly we see that we should spend our capacity of things-that-grow most around the time we expect AGI to appear. For the 2040 and 2050 timelines, this implies spending very little on things that depreciate, up to around 3% a year. For 2030 timelines, we should be spending between 5 and 10% of our capacity each year on ‘crunching’ for the arrival of AGI. Further, for all results, we begin maximum crunching *after  the*modal AGI arrival date, which is understandable while the rate of growth of the movement is greater than the rate of decrease in probability of AGI (times the discount factor).

This result is relatively sensitive to the probability we think AGI will appear in the next few years. We fit a log-normal distribution to the AGI timeline with ![p(0)=0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/cdb8a56068a64ab4f77abf9be458b860.png "Rendered by QuickLaTeX.com") which leads to ![p(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e047cb96b673a8d692da97b97f78cede.png "Rendered by QuickLaTeX.com") being small for the next few years. Considering a probability distribution that gave some weight to AGI in the next few years would inevitably imply a higher initial spending rate,  though likely  a similar overall spending schedule in sufficiently many years time.

|  |  |  |  |
| --- | --- | --- | --- |
|  | *Median AGI arrival* | | |
| *Difficulty of AGI success* | 2030[85](#easy-footnote-bottom-85-8199 "50% AGI by 2030, 75% by 2040") | 2040[86](#easy-footnote-bottom-86-8199 "50% AGI by AGI by 2040, 75% by 2060") | 2050[87](#easy-footnote-bottom-87-8199 "50% AGI by 2050, 75% by 2075") |
| Easy[88](#easy-footnote-bottom-88-8199 "50% AGI success if we spent half our capacity for one year, <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-2f8a1d36a3200bdfebbabc2d972bb6fb_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#107;&#97;&#112;&#112;&#97;&#32;&#61;&#32;&#53;\" title=\"Rendered by QuickLaTeX.com\" height=\"13\" width=\"42\" style=\"vertical-align: 0px;\"/>") |  |  |  |
| Medium[89](#easy-footnote-bottom-89-8199 "25% AGI success if we spent half our capacity for one year, <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-17de919c26b32705d2a3a8b98cd21350_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#107;&#97;&#112;&#112;&#97;&#32;&#61;&#32;&#51;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"43\" style=\"vertical-align: 0px;\"/>") |  |  |  |
| Hard[90](#easy-footnote-bottom-90-8199 "10% AGI success if we spent half our capacity for one year <img src=\"https://longtermrisk.org/wp-content/ql-cache/quicklatex.com-d5b2dd1961bd4427f534216846ca6b4d_l3.png\" class=\"ql-img-inline-formula quicklatex-auto-format\" alt=\"&#92;&#107;&#97;&#112;&#112;&#97;&#32;&#61;&#49;\" title=\"Rendered by QuickLaTeX.com\" height=\"12\" width=\"42\" style=\"vertical-align: 0px;\"/>") |  |  |  |

### Limitations

Many of the limitations we describe apply to both models.

For example, there is no exogenous increase in ![C(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/515955a3ad1ae2fa344a290c1aa9e110.png "Rendered by QuickLaTeX.com") which we may expect if other actors' work on AI risk at some time in the future. One could, for example, adjust ![c(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5016c6770e3f9e0f3519394086c4699a.png "Rendered by QuickLaTeX.com") such that spending on direct work receives more units of ![C(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/515955a3ad1ae2fa344a290c1aa9e110.png "Rendered by QuickLaTeX.com") per unit spending in the future due to others' also working on the problem.

Like the first model, our work and AI capabilities are independent. One could, again, use ![c(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5016c6770e3f9e0f3519394086c4699a.png "Rendered by QuickLaTeX.com") to model direct work becoming cheaper as time goes on and new AI capabilities are developed.

## Full results from the nine cases

|  |  |  |
| --- | --- | --- |
|  |  |  |
|  |  |  |
|  |  |  |

# Robust spending schedules by Monte Carlo simulation

*Added 2022-11-29, see discussion*[*here*](https://forum.effectivealtruism.org/posts/mLqKcYahP5nbjK9ir/tristan-cook-s-shortform?commentId=So4dTJWomiE975T7m)

Here I consider the most **robust** spending policies and supposes uncertainty over nearly all parameters in the main model[91](#easy-footnote-bottom-91-8199 "Inputs that are not considered include: historic spending on research and influence, the rate at which the real interest rate changes, the post-fire alarm returns are considered to be the same as the pre-fire alarm returns."), rather than point-estimates. I  find that **the community’s current spending rate on AI risk interventions is too low**.

My distributions over the the model parameters imply that

* Of all *fixed*spending schedules (i.e. to spend X% of your capital per year[92](#easy-footnote-bottom-92-8199 "And supposing a 50:50 split between spending on research and influence")), the best strategy is to spend 4-6% per year.
* Of all *simple*spending schedules that consider two regimes: now until 2030, 2030 onwards, the best strategy is  to spend ~8% per year until 2030, and ~6% afterwards.

I recommend entering your own distributions for the parameters in the Python notebook [here](https://colab.research.google.com/drive/1JJU_P9A-3XXvyUo0DyoR6q-PDmr_2fPf?usp=sharing)[93](#easy-footnote-bottom-93-8199 "This notebook is  less user-friendly than the notebook used in the main optimal spending result (though not <em>un</em> user friendly)  - let me know if improvements to the notebook would be useful for you."). Further, these preliminary results use few samples: more reliable results would be obtained with more samples (and more computing time).

I allow for post-fire-alarm spending (i.e., we are certain AGI is soon and so can spend some fraction of our capital). Without this feature, the optimal schedules would likely recommend a greater spending rate.

![](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/472879a3016d366f40beeb1910088d32.png)

Fixed spending rate. See [here](https://docs.google.com/document/d/1gNMy900q2sP0tFasKi2jnbIlwQGcSOxPKg_obNXWVAk/edit) for the distributions of utility for each spending rate.

![](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/efdf85461f1b4d314cee2edc02bd58aa.png)

Simple - two regime - spending rate

|  |
| --- |
|  |
| The results from a simple optimiser[94](#easy-footnote-bottom-94-8199 "The intermediate steps of the optimiser are <a href=\"https://docs.google.com/document/d/1GQdqsBhPgmA8DNy9Ed25zlmunxhxxYljpqaQhKz8G6E/edit\" target=\"_blank\" rel=\"noopener\">here</a>."), when allowing for four spending regimes: 2022-2027, 2027-2032, 2032-2037 and 2037 onwards. This result should not be taken too seriously: more samples should be used, the optimiser runs for a greater number of steps and more intervals used. As with other results, this is contingent on the distributions of parameters. |

### Some notes

* The system of equations - describing how a funder’s spending on AI risk interventions change the probability of AGI going well - are unchanged from the main model.
* This version of the model randomly generates the real interest, based on user inputs. So, for example, one’s capital can go down.

![](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/7f85c11df4c99b9e5764ffd4fb2320bd.png)

n example real interest function ![r(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/1cf8825a7a726a6ee93c73d15e987e67.png "Rendered by QuickLaTeX.com"), cherry picked to show how our capital can go down significantly. See [here](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/7a399b67e1cf8d731c485db0e8342be0.jpg) for 100 unbiased samples of ![r(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/1cf8825a7a726a6ee93c73d15e987e67.png "Rendered by QuickLaTeX.com")

![](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/7defabd306b7736e922891388ba00bf0.jpg)

Example probability-of-success functions. The filled circle indicates the current preparedness and probability of success.

![](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/9de118a8c0b33e83dca647a928fbe6f1.png)

Example competition functions. They all pass through (2022, 1) since the competition function is the *relative* cost of one unit of influence compared to the current cost.

This short extension started due to a conversation with David Field and comment from Vasco Grilo; I’m grateful to both for the suggestion.

# Author contributions

Tristan and Guillaume defined the problem, designed the model and its numerical resolution, interpreted the results, wrote and reviewed the article. Tristan coded the Python notebook and carried out the numerical computations with feedback from Guillaume. Tristan designed, coded, solved the alternate model and interpreted its results.

# Acknowledgements

We’d both like to thank Lennart Stern and Daniel Kokotajlo for their comments and guidance during the project. We’re grateful to John Mori for comments.

Guillaume thanks the SERI summer fellowship 2021 where this project started with some excellent mentorship from Lennart Stern, the CEEALAR organisation for a stimulating working and living environment during the summer 2021 and the CLR for providing funding to support part-time working with Tristan to make substantial progress on this project.

---



1. [Todd (2021)](https://80000hours.org/2021/07/effective-altruism-growing/) claims 1% donated per year for the whole effective altruism community. The Open Philanthropy project spent [\$80m in 2021 on AI risk interventions](https://docs.google.com/spreadsheets/d/1XpWNGyho_kkSkVlMsqnddrhnEYW7MRQBmLX0wITYxGQ/edit?usp=sharing). In 2021 they [had approximately \$17.8b committed](https://www.forbes.com/profile/dustin-moskovitz/?sh=9ba79cf1dd34). Supposing that at least one sixth of their budget is committed to AI risk interventions, this gives a spending rate of at most 2.6%.  The FTX Future Fund has granted [around \$31m on AI risk interventions](https://docs.google.com/spreadsheets/d/1CI-8rUgjU6s63tUnqCk94KlbojEkyheFiHXliT6dE8M/edit#gid=0) since starting over a year ago. Supposing at least one tenth of their budget is committed to AI risk interventions, this gives a spending rate of at most \$31m/([\$16,600m](https://www.forbes.com/profile/sam-bankman-fried/?sh=2eb301b74449) /10) = 1.9% per year. For the AI s-risk community, the figure is around 3%.
2. This is true when supposing a 4% constant spending rate, which is an overestimate of current spending but maybe underestimating future spending.
3. The second model requires us to split activities into capacity growing and capacity shrinking that increase our probability of success whereas the first model talks concretely about the spending rate of money.
4. The values chosen are discussed [here](#appendix).
5. 25% AGI by 2027, 50% 2030
6. 50% AGI by AGI by 2040, 75% by 2060
7. 50% AGI by 2050, 75% by 2075
8. The easy case is operationalised by the inputs in the model:  Probability of success if AGI this year = 25%, and $l=0.20$. The $l$ term describes the steepness of the s-shaped curve of success.
9. The “break even line” is the maximum rate at which the funder can spend and still have their money increase.
10. Probability of success if AGI this year = 10%, and $l=0.10$
11. p(success if AGI this year) = 4%, and $l=0.05$
12. This is a lower bound for two reasons: first, there may be spending schedules better than those that we present. Second, we calculate the utility of the 4% strategy for an arbitrarily long time horizon whereas we compute the optimal spending schedules within the year 2100.
13. *Added post-publication on 2022-11-29*
14. We use semi-arbitrary units of ‘quality-adjusted relevant effort units’. We use ‘quality-adjusted’ to imply that an expert's hour of contribution is worth more than a novice’s hour of contribution. We use ‘relevant’ to discount any previously acquired research or influence that is no longer useful. We use ‘effort units’ to mostly account for the time that people have put into working on something.
15. We give a more complete account in the technical description. In short, the solution is given as a numerical solution to an expanded set of differential equations.
16. The opposite is also plausible if AI risk becomes increasingly salient.
17. Taking $\delta=0.4$
18. Taking $\delta=0.2$
19. We see that even with practically no money we still achieve some utility. This is because both (1) the probability of success is non-zero when we have no research or influence, and (2) we already have some research and influence that will depreciate over time with no further spending.
20. $\eta\_R = 0.15, \eta\_I = 0.1$
21. As discussed in the appendix, this is $\eta\_R =0.3 , \eta\_I = 0.2$
22. $\eta\_R =0.45 , \eta\_I = 0.3$
23. This weight-adjusted is the $\gamma$ term in the [constant elasticity of substitution function](https://en.wikipedia.org/wiki/Constant_elasticity_of_substitution)
24. This is done by increasing $\rho$ up to 1.
25. This is due to our choice of $\gamma$
26. In the sense that (1) it depreciates at a lower rate (2) there are lower diminishing marginal returns.
27. At a high enough spending rate one marginal unit of influence is cheaper than one marginal unit of influence due to diminishing marginal returns
28. We take $\rho=-10$
29. We take $\rho = 0.001$
30. This has $\rho=0.3$
31. This is $\rho=1$
32. Probability of success if AGI is this year is 0.1%, and steepness $l=0.1$
33. $\rho =0.8$
34. This is $\rho$ is low, perhaps less than or equal to zero.
35. We take $\rho \approx 0$, so this is the Cobb-Douglas production function
36. Similar to how $c(t)$ makes influence more expensive over time.
37. We have $r=0.10, \, \eta\_R = 0.3, \,  M\_0 = 4000$
38. 50% AGI by 2030, 75% by 2040
39. 50% AGI by AGI by 2040, 75% by 2060
40. 50% AGI by 2050, 75% by 2075
41. 50% AGI success if we spent half our capacity for one year, $\kappa = 5$
42. 25% AGI success if we spent half our capacity for one year, $\kappa = 3$
43. 10% AGI success if we spent half our capacity for one year $\kappa =1$
44. Inputs that are not considered include: historic spending on research and influence, the rate at which the real interest rate changes, the post-fire alarm returns are considered to be the same as the pre-fire alarm returns.
45. And supposing a 50:50 split between spending on research and influence
46. This notebook is  less user-friendly than the notebook used in the main optimal spending result (though not *un* user friendly)  - let me know if improvements to the notebook would be useful for you.
47. The intermediate steps of the optimiser are [here](https://docs.google.com/document/d/1GQdqsBhPgmA8DNy9Ed25zlmunxhxxYljpqaQhKz8G6E/edit).
48. [Todd (2021)](https://80000hours.org/2021/07/effective-altruism-growing/) claims 1% donated per year for the whole effective altruism community. The Open Philanthropy project spent [$80m in 2021 on AI risk interventions](https://docs.google.com/spreadsheets/d/1XpWNGyho_kkSkVlMsqnddrhnEYW7MRQBmLX0wITYxGQ/edit?usp=sharing). In 2021 they [had approximately $17.8b committed](https://www.forbes.com/profile/dustin-moskovitz/?sh=9ba79cf1dd34). Supposing that at least one sixth of their budget is committed to AI risk interventions, this gives a spending rate of at most 2.6%.  The FTX Future Fund has granted [around $31m on AI risk interventions](https://docs.google.com/spreadsheets/d/1CI-8rUgjU6s63tUnqCk94KlbojEkyheFiHXliT6dE8M/edit#gid=0) since starting over a year ago. Supposing at least one tenth of their budget is committed to AI risk interventions, this gives a spending rate of at most $31m/([$16,600m](https://www.forbes.com/profile/sam-bankman-fried/?sh=2eb301b74449) /10) = 1.9% per year. For the AI s-risk community, the figure is around 3%.
49. This is true when supposing a 4% constant spending rate, which is an overestimate of current spending but maybe underestimating future spending.
50. The second model requires us to split activities into capacity growing and capacity shrinking that increase our probability of success whereas the first model talks concretely about the spending rate of money.
51. The values chosen are discussed [here](#appendix).
52. 25% AGI by 2027, 50% 2030
53. 50% AGI by AGI by 2040, 75% by 2060
54. 50% AGI by 2050, 75% by 2075
55. The easy case is operationalised by the inputs in the model:  Probability of success if AGI this year = 25%, and ![l=0.20](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/ad9391dae0c19a58fbc19189181e18a1.png "Rendered by QuickLaTeX.com"). The ![l](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/7324b4b7812a0f0ba406e36ff76d8cc9.png "Rendered by QuickLaTeX.com") term describes the steepness of the s-shaped curve of success.
56. The “break even line” is the maximum rate at which the funder can spend and still have their money increase.
57. Probability of success if AGI this year = 10%, and ![l=0.10](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/9aca2cd7fdfc46bb1ac563b5cd246fe9.png "Rendered by QuickLaTeX.com")
58. p(success if AGI this year) = 4%, and ![l=0.05](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/3c3f8754f3bb7d49acad08c667bb6dd4.png "Rendered by QuickLaTeX.com")
59. This is a lower bound for two reasons: first, there may be spending schedules better than those that we present. Second, we calculate the utility of the 4% strategy for an arbitrarily long time horizon whereas we compute the optimal spending schedules within the year 2100.
60. *Added post-publication on 2022-11-29*
61. We use semi-arbitrary units of ‘quality-adjusted relevant effort units’. We use ‘quality-adjusted’ to imply that an expert's hour of contribution is worth more than a novice’s hour of contribution. We use ‘relevant’ to discount any previously acquired research or influence that is no longer useful. We use ‘effort units’ to mostly account for the time that people have put into working on something.
62. We give a more complete account in the technical description. In short, the solution is given as a numerical solution to an expanded set of differential equations.
63. The opposite is also plausible if AI risk becomes increasingly salient.
64. Taking ![\delta=0.4](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/329d7978c1c3e6c22b70162d26e2f99a.png "Rendered by QuickLaTeX.com")
65. Taking ![\delta=0.2](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/1a5224d0d06afa36ec7426e07e839dff.png "Rendered by QuickLaTeX.com")
66. We see that even with practically no money we still achieve some utility. This is because both (1) the probability of success is non-zero when we have no research or influence, and (2) we already have some research and influence that will depreciate over time with no further spending.
67. ![\eta_R = 0.15, \eta_I = 0.1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/35e41d0a1552371770b0422034bf8a40.png "Rendered by QuickLaTeX.com")
68. As discussed in the appendix, this is ![\eta_R =0.3 , \eta_I = 0.2](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/670456397173080dd38a6262f9296b6a.png "Rendered by QuickLaTeX.com")
69. ![\eta_R =0.45 , \eta_I = 0.3](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/282ff7edce5f27423ef4a277d6114fd4.png "Rendered by QuickLaTeX.com")
70. This weight-adjusted is the ![\gamma](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/dd6823af35cc1bee47eb056352004b63.png "Rendered by QuickLaTeX.com") term in the [constant elasticity of substitution function](https://en.wikipedia.org/wiki/Constant_elasticity_of_substitution)
71. This is done by increasing ![\rho](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/755b4a0f35e8d342d0840e253eea4fc3.png "Rendered by QuickLaTeX.com") up to 1.
72. This is due to our choice of ![\gamma](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/dd6823af35cc1bee47eb056352004b63.png "Rendered by QuickLaTeX.com")
73. In the sense that (1) it depreciates at a lower rate (2) there are lower diminishing marginal returns.
74. At a high enough spending rate one marginal unit of influence is cheaper than one marginal unit of influence due to diminishing marginal returns
75. We take ![\rho=-10](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/f2bfb4cc48a7fbc473f5307b2a09cade.png "Rendered by QuickLaTeX.com")
76. We take ![\rho = 0.001](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/4f921406aaa5c122df70077bd67e51d3.png "Rendered by QuickLaTeX.com")
77. This has ![\rho=0.3](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/70d52f100ec9bf4a50a66c311c6e7421.png "Rendered by QuickLaTeX.com")
78. This is ![\rho=1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/47edccc9464d102e40ab0d658fdca865.png "Rendered by QuickLaTeX.com")
79. Probability of success if AGI is this year is 0.1%, and steepness ![l=0.1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/39e4d05f68b7851791bbf28ddfcc53c1.png "Rendered by QuickLaTeX.com")
80. ![\rho =0.8](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/c21d0a7d500267d63bcccca9b0c9dc40.png "Rendered by QuickLaTeX.com")
81. This is ![\rho](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/755b4a0f35e8d342d0840e253eea4fc3.png "Rendered by QuickLaTeX.com") is low, perhaps less than or equal to zero.
82. We take ![\rho \approx 0](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/0008556c5fa81525e639c71bc84455e2.png "Rendered by QuickLaTeX.com"), so this is the Cobb-Douglas production function
83. Similar to how ![c(t)](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5016c6770e3f9e0f3519394086c4699a.png "Rendered by QuickLaTeX.com") makes influence more expensive over time.
84. We have ![r=0.10, \, \eta_R = 0.3, \,  M_0 = 4000](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/5e7cc844889d6d6cfb22473736f6a078.png "Rendered by QuickLaTeX.com")
85. 50% AGI by 2030, 75% by 2040
86. 50% AGI by AGI by 2040, 75% by 2060
87. 50% AGI by 2050, 75% by 2075
88. 50% AGI success if we spent half our capacity for one year, ![\kappa = 5](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/f86262a4e78f19cddf05c1862c52570a.png "Rendered by QuickLaTeX.com")
89. 25% AGI success if we spent half our capacity for one year, ![\kappa = 3](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/25e21c550cd461315a0cfa4b97ffe1b6.png "Rendered by QuickLaTeX.com")
90. 10% AGI success if we spent half our capacity for one year ![\kappa =1](ai-leaders-insights/安全治理与未来/时间线与展望/保守派预测/images/e0fcf4fea3ce5a5497443e633c1a6e1a.png "Rendered by QuickLaTeX.com")
91. Inputs that are not considered include: historic spending on research and influence, the rate at which the real interest rate changes, the post-fire alarm returns are considered to be the same as the pre-fire alarm returns.
92. And supposing a 50:50 split between spending on research and influence
93. This notebook is  less user-friendly than the notebook used in the main optimal spending result (though not *un* user friendly)  - let me know if improvements to the notebook would be useful for you.
94. The intermediate steps of the optimiser are [here](https://docs.google.com/document/d/1GQdqsBhPgmA8DNy9Ed25zlmunxhxxYljpqaQhKz8G6E/edit).

---

*爬取时间: 2025-11-28 21:59:58*
