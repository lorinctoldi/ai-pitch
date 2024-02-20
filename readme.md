Task in hand:
Take a list of issues and summarise them. 
Additional positives:
- option for sorting 
- option for length

Main question:
Summarise ONLY?

1. NO:
General-purpose AI

pro:
- no config
- good docs
- easy to blame
- prompt engineering

 setbacks: 
- “halucination” (issues from training, evaluations….) (f.e. 100 issues -> 100 sentences min.), 
- lack of reliability, 
- …transparency, 
- …controllability, 
- price
- hard (impossible) to replace (e.g. OpenAI 86bUSD > Diligent 7bUSD)
- does not sound impressive

examples:
- vertex
- chatgpt (enterprise
- gemini
- amazon products
- …

2. YES
NOT general-purpose:

questions: (I) How to summarize (approach, tool)? How to rank / evaluate (and why)? How to identify categories / cases (and why)?



(I) How to summarise? 
Summarisation ai (https://dashboard.cohere.com/playground/summarize)

Pros: 
- The “Right” tool (reliable, less complex, …)
- options (length, format, model, EXTRACTIVENESS, …)
- Reliable
- 1$ / 1M input tokens & 2$ / 1m output token

Cons: 
- Can’t sort or evaluate (most of them)

Can’t sort or evaluate: 
Not guaranteed the list of issues is ranked from most important, linear time line. 
-> (- Tell me about a movie! - XY had a brown shirt….) Start from the most important!
Can’t sort: has to see all issues or loose some random (based on summary length f.e.)



(II) How to rank / evaluate (and why)

Can’t sort from costume, or missing issue type / severity! (Brutal ? Severe ? High)

sentiment evaluation (key concepts)
- Scoring (words of sentences) with pos./neg values. (“nice” -> +x, “hate” -> -y);
- score / comparative / calculations / tokens / negatives - positives
- ML? No & Yes! (https://connexun.com/demos/text-analysis-sentiment-evaluation)

Pros:
- Easy to understand, modify
- Quick as hell
- Key for sorting
- Can work with missing data (scoring out)

Cons:
- if local, must “””train””” (generate via. GPTs)
- …

(III) How to identify categories / cases (and why)?
~sentiment evaluation:
Predefined categories. (IT, HR, Supplies, …) 
Tokens are not neg./pos., but (0.x category[0], 0.y category[1], ….).
Highest scored category shall be used. 

Based on severity rank, and category: Limit and sort the sent out data.


