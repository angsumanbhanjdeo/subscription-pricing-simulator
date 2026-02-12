SUBSCRIPTION PRICING SIMULATOR
Model Documentation, Logic & Plain-English Guide
Angsuman Bhanjdeo  | Senior Commercial & Trading Performance Manager, Sky UK
February 2026

⚠  IMPORTANT DISCLAIMER:  This model represents my personal thinking on subscription pricing frameworks. It does NOT reflect the actual pricing processes, methodologies, or internal systems in any places that I have worked. Every company has its own rigorous, proprietary approach to pricing decisions involving teams of specialists, legal, regulatory, and competitive considerations. This is a personal intellectual exercise — a framework I would consider if I were building a subscription business from the ground up.

1. Why I Built This
Having worked in subscription businesses, I've always been fascinated by a deceptively simple question: what is an objective way to approach pricing decisions.
On the surface, it sounds obvious — charge more, earn more. But the reality is far more nuanced. Raise prices too aggressively and you lose customers. Raise them too little and you leave money on the table. Get it wrong either way, and the business suffers.
What struck me is that in most organisations, pricing decisions are still made largely through gut instinct, competitive benchmarking, or finance-led cost-plus models. Very few teams attempt to model the interplay between price, customer behaviour, and long-term revenue in a dynamic way.
This simulator is my attempt to build a framework that brings together the key variables I believe any commercial leader in a subscription business should be looking at — simultaneously, not in isolation. I want to stress: real-world pricing also requires competitive intelligence, regulatory considerations, brand positioning, customer segmentation, and market timing. This model is a starting point for structured thinking, not a replacement for the full picture.
2. Glossary of Key Terms
Before we get into the model, here are the key terms explained as simply as possible. I have included the technical definition too, but the simplified definition is what actually matters.

Churn Rate	Simplified Definition:  The percentage of your customers who leave every month. If you have 1,000 customers and 30 leave in January, your churn rate is 3%.
Technical:  Monthly attrition rate: (customers lost ÷ customers at start of period) × 100.


LTV	Simplified Definition:  Customer Lifetime Value — how much money you'll make from one customer before they cancel. If they pay £10/month and stay for 20 months, their LTV is roughly £200.
Technical:  LTV = (Average Revenue per User − Cost per User) ÷ Monthly Churn Rate.

Price Elasticity	Simplified Definition:  How sensitive your customers are to price changes. If you raise prices by 10% and lots of people leave, demand is 'elastic' (sensitive). If almost nobody leaves, demand is 'inelastic' (not sensitive).
Technical:  Price Elasticity of Demand (PED) = % change in quantity demanded ÷ % change in price. Values between -1 and 0 are inelastic; below -1 is elastic.

Break-even Churn	Simplified Definition:  The maximum number of customers you can afford to lose before the price increase actually hurts you. If your new price is 10% higher but 15% of customers leave, you're worse off.
Technical:  Break-even subscriber loss = Current Revenue ÷ New Price − Current Subscribers. Expressed as a percentage of the subscriber base.

P&L	Simplified Definition:  Profit & Loss — basically your business's scorecard. Revenue coming in, costs going out, what's left over is profit. In subscription businesses, improving P&L usually means growing revenue and reducing churn simultaneously.
Technical:  Income Statement showing revenues, costs, and resulting margin over a defined period.

GMV	Simplified Definition:  Gross Merchandise Value — the total sales value flowing through a platform. For a marketplace like Amazon, this is the total value of everything sold, before any fees or deductions.
Technical:  Total value of transactions facilitated by a platform, before returns, cancellations, or platform fees.

ARPU	Simplified Definition:  Average Revenue Per User — how much each customer pays you on average per month. If you have 500,000 customers and make £6.5M per month, your ARPU is £13.
Technical:  ARPU = Total Monthly Revenue ÷ Total Active Subscribers.

Cohort Model	Simplified Definition:  A way of tracking groups of customers who joined at the same time to see how they behave over months. It's like tracking Class of 2022 separately from Class of 2023, so you can see whether newer customers churn faster or slower.
Technical:  Longitudinal analysis of customer groups segmented by acquisition period, tracking retention and revenue metrics over time.




3. How the Model Works
The model is built around five core inputs and produces five types of output. Here's the logic behind each.
3.1 The Five Inputs
Current Monthly Price  (£)
The starting point. Everything is relative to this. The model calculates the impact of any proposed change as a percentage increase or decrease from here.
Total Subscribers
How many paying customers you currently have. This directly determines your revenue baseline. The model tracks how this number evolves month by month under both old and new pricing scenarios.
Monthly Churn Rate  (%)
Your base churn — what percentage of customers leave naturally each month, even without a price change. This is your single most important metric in a subscription business. A 1% difference in monthly churn translates to millions in lost revenue over a year at scale.
New Subscriber Acquisition (per month)
How many new customers you add each month. The model assumes this stays constant after a price change — in reality, a significant price rise might reduce acquisition too, but that's a secondary effect and varies greatly by marketing strategy and market conditions.
Cost per Subscriber  (£/month)
The variable cost of serving one customer for one month — content costs, infrastructure, customer service allocation, etc. This is needed to calculate true margin and LTV, not just revenue.
3.2  The Pricing Decision Inputs
Proposed Price Change  (%)
The percentage increase or decrease you are considering. The model runs the full scenario from -30% (aggressive discount) to +50% (significant increase) and highlights where on that curve the current proposed change sits.
Price Elasticity of Demand
This is the most important — and most misunderstood — input in the model. It represents how sensitive your specific customer base is to a price change.
In simple terms: if you raise prices by 10% and you expect to lose 8% of customers as a result, your elasticity is roughly -0.8. The model lets you set this based on your knowledge of your market.
Typical ranges from research and industry data:
–	Streaming / media (Netflix, Disney+, Sky): -0.5 to -1.2
–	SaaS with low switching costs: -1.0 to -2.0
–	Essential software with high switching costs: -0.1 to -0.4
–	Commodity subscription (easily replaced): -2.0 to -3.0

💡  MY VIEW:  The elasticity figure is where most pricing models fall down. Companies often assume their customers are more price-inelastic than they actually are, because their pricing is rarely tested rigorously. In my experience, subscription customers in competitive markets are more price-sensitive than businesses like to admit — especially for products that feel discretionary rather than essential.
3.3  What the Model Calculates
Subscriber Impact
Using the elasticity figure, the model estimates the incremental churn caused by the price change. This is applied on top of the natural base churn rate to give a new, higher churn rate under the new pricing scenario.
Formula: Churn uplift = Elasticity × Price change %  →  New churn rate = Base churn + (Base churn × Churn uplift)
Revenue Impact
The model compares monthly revenue under both scenarios. It shows not just whether total revenue goes up, but the waterfall breakdown — how much you gain from charging more per subscriber, and how much you lose from the customers who leave.
LTV Change
Because LTV depends on both the margin per customer AND how long they stay, a price change affects LTV in two directions at once: higher price improves margin per month, but higher churn reduces how many months you keep them. The model shows you the net effect.
Break-Even Analysis
This answers the question: how many customers can you afford to lose before you wish you hadn't raised prices? This is the most practically useful output for a commercial decision — it gives you a risk tolerance threshold.
12-Month Projection
The model runs a month-by-month simulation over 12 months, compounding the churn and acquisition effects. This shows that even if month 1 looks positive, the churn effect can compound over time and erode the initial revenue gain.
4. Assumptions & Limitations
📋  READ THIS SECTION:  No model is perfect. Being transparent about what this model assumes — and where it falls short — is critical for using it responsibly.

4.1  What the Model Assumes
▸	Elasticity is constant across the entire subscriber base.
–	Reality: Different customer segments (premium vs basic, new vs long-tenure) have very different price sensitivities. A full model would segment these separately.
▸	Acquisition rate stays the same after a price change.
–	Reality: A higher price point may reduce conversion on acquisition campaigns. The model does not capture this secondary effect.
▸	Churn uplift from pricing is immediate (happens in month 1).
–	Reality: Churn from a price change often spikes at the first billing cycle after the change and then normalises. The shape of the churn curve matters.
▸	All subscribers are on the same price.
–	Reality: Most businesses have multiple tiers, grandfathered pricing, promotional subscribers, and bundled customers who will behave differently.
▸	Costs remain fixed per subscriber.
–	Reality: Economies of scale mean cost per subscriber can change as the base grows or shrinks.
4.2  What This Model Does NOT Replace
▸	Competitive analysis: What are rivals charging? What happens if a competitor undercuts you after your increase?
▸	Customer research: What do customers actually say about value and willingness to pay?
▸	Regulatory and legal review: Price changes in regulated industries require specific approvals.
▸	Brand impact assessment: A perceived 'unfair' price rise can have reputational consequences beyond just churn.
▸	Segmentation analysis: Heavy users, casual users, and at-risk customers need different treatment.
▸	Competitive and macroeconomic timing: Raising prices during a cost-of-living crisis, for example, carries different risks than in a benign economic environment.

🔑  THE BIG PICTURE:  In practice, pricing decisions in large subscription businesses are made by cross-functional committees — commercial, finance, product, legal, marketing, and customer insight teams all have a seat at the table. This model is the kind of framework I would bring to that conversation as a starting point for structured, quantified discussion. It is not the end of the analysis — it is the beginning.
5. How I Would Use This in Practice
If I were running commercial strategy for a subscription business and we were considering a price change, here is how I would deploy this framework:
Step 1: Establish Your Elasticity Estimate
Before running any scenarios, the most important work is estimating your actual price elasticity. You can do this through: historical price test data, survey-based willingness-to-pay research (Van Westendorp or Gabor-Granger methods), or regression analysis on past price changes. Most businesses have some of this data — it just isn't synthesised into a single figure.
Step 2: Run Multiple Scenarios
Don't just model your target price. Run at least three: a conservative case (small increase, low elasticity), a base case (target increase, expected elasticity), and a stress case (target increase, higher elasticity than expected). The gap between scenarios tells you your risk exposure.
Step 3: Focus on the Break-Even Number
The single most useful output is the break-even churn figure. If you need to lose fewer than 8% of customers to still come out ahead, and your best estimate is that you'll lose 4-5%, the decision is relatively straightforward. If break-even is 3% but your estimate is 5-8%, the margin of safety is too thin.
Step 4: Layer In What the Model Misses
Once the quantitative case is established, bring in competitive positioning, customer research, timing, and segmentation. A good number on a model is a necessary condition for a pricing decision — it is not a sufficient one.
Step 5: Design the Change Thoughtfully
How you raise prices matters as much as whether you raise them. Grandfathering loyal customers, bundling new features with the increase, offering annual plans at a locked price, and giving advance notice all affect the actual churn outcome vs the modelled expectation.
6. Sources & Further Reading
The concepts in this model draw from established economic theory and commercial strategy literature. For those who want to go deeper:
▸	Simon, H. & Fassnacht, M. (2019). Price Management. Springer — widely considered the definitive commercial pricing textbook.
▸	Anderson, E.T. & Simester, D. (2003). Effects of $9 Price Endings on Retail Sales. Quantitative Marketing and Economics.
▸	Van Westendorp, P.H. (1976). Price Sensitivity Meter — the foundational methodology for consumer willingness-to-pay research.
▸	Tzuo, T. (2018). Subscribed: Why the Subscription Model Will Be Your Company's Future. Portfolio/Penguin — excellent practitioner-level view on subscription economics.
▸	Gopinath, G. et al. — IMF research on price stickiness and consumer response in service markets.

A Final Note
Building this model was a personal exercise in applied commercial thinking. The underlying question — how do you balance short-term revenue optimisation against long-term customer relationships — is one I find genuinely fascinating, and one that I believe doesn't get enough rigorous quantitative treatment in most commercial teams.
Pricing is one of the highest-leverage levers a business has. A 1% improvement in price, sustained across a large subscriber base, can be worth more than a 10% improvement in cost efficiency. Yet most businesses under-invest in pricing capability relative to other commercial functions.
I hope this model, and the thinking behind it, is useful. Feedback is always welcome.

Angsuman Bhanjdeo  |  angsumanbhanjdeo@gmail.com  |  linkedin.com/in/angsumanbhanjdeo
