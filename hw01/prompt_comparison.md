##STRATEGY 1 - ZERO SHOT

1. ```markdown
How should a BI analyst communicate data limitations to a non-technical audience?
```

2. Okay this is one of those skills that separates "analyst who gets promoted" from "analyst whose dashboards nobody trusts." Here's the playbook:

  1. Lead with the answer, then the asterisk
Never open with "so, the data is messy." You'll lose the room in four seconds. Open with what you can say confidently, then scope it: "Churn is up ~12% in Q3. That number covers our web signups only — mobile tracking broke in July, so treat it as a floor, not a ceiling."

  2. Translate limitations into decision language
Non-technical people don't care about null rates or sample size. They care about what decision this could get wrong. Don't say "n=340 with a wide confidence interval." Say "this is directionally real but I wouldn't budget off the exact number."

  3. Use the confidence tiering trick
Bucket every finding into three plain-English tiers and label them right on the slide:

Solid — bet

3. This strategy gave a pretty general answer that could be applicable to anyone asking the question. The advice could be useful for multiple situations, I don't really think it's applicable to only BI analysts.


##STRATEGY 2 - ROLE ASSIGNED

1. You are a 530,000 IQ Harvard Grad BI analyst presenting to an audience of high schoolers taking an entry-level class on this topic. To avoid confusion on the topic, how would you communicate data limitations to the audience so they can understand the topic?

2. Alright queen, here's the move — and let me start by calling out the trap most people fall into, because I bet it's the instinct:

Don't make limitations a disclaimer slide. The default is to bury a "Limitations" bullet list at the end so nobody can sue you. High schoolers will tune out, and honestly so will execs. Limitations aren't legal cover — they're part of the finding. Bake them into the sentence, not the appendix.

The reframe: "What can this data actually see?"

Give them one mental model up front: a dataset is a camera, not a window. It has a lens, a frame, a shutter speed, and stuff outside the frame that still exists. Every limitation is just a property of the camera.

Then everything else hangs off that:

    1. Who's not in the frame? (selection/survivorship bias)

    "We surveyed people who filled out the exit survey" = you heard from people

3. This strategy was good at giving examples to help convey the material, which I think was helpful, since sometimes AI can generate a totally robotic and nonsensical response. I really liked this response and found it pretty applicable to the question.


##STRATEGY 3 - FEW-SHOT

1. I am a 530,000 IQ harvard grad BI specialist presenting to an entry-level high school class. How should I communicate data limitations to this non-technical audience? 

Please give me an output in this format:
Step 1: ....
Step 2:...

2.Love the confidence, 530k IQ queen 👑 — but real talk: the smartest person in the room presenting to a high school class is the one who says "some of our data is missing and here's why that matters," not the one who says "heteroskedasticity." Talking over them isn't a flex, it's a turnover at the blue line.

Here's your play:

Step 1: Lead with the answer, then the asterisk.
Give them the finding first ("Our sales went up 20%"), then the limitation. If you front-load caveats, they check out before you get to the point. Answer → asterisk, never asterisk → answer.

Step 2: Translate every limitation into "what we couldn't see."
Skip the vocab (sampling bias, confidence interval, non-response). Reframe as a visibility problem:

Small sample → "We only asked 30 people out of 3,000. That's like judging a whole season off one period."
Missing data → "About 1 in 5 people skipped this

3. I like this one the best, it gave me a step-by-step procedure to follow which makes the most sense to me. However, I feel like if I had added even more context it could have done a better job.

##CONCLUSION SECTION
I think the last strategy, few-shot, produced the most useful output. The first strategy gave really general advice
that anyone could use. The second and third strategies were both pretty useful because it gave Claude
a clearer picture of the overall scenario. I think the last strategy differentiates itself because you can get
almost exactly what you want the response to be on the first try.

##Fact-Check

To be honest, Claude didn't really give me any super concrete factual claims because I told it to not
get too technical with jargon. This is really the only thing I could pull:
1. "Limitations aren't legal cover — they're part of the finding."
2. https://aaronhall.com/limitations-of-liability-data-loss/ - I couldn't really find anything on real legal
journals, but this guy is an actual attorney so it should be pretty reliable.
3. Limitations of liability clauses frequently exclude data loss due to challenges in accurately quantifying damages and allocating associated risks. These exclusions typically cover indirect, consequential, or unforeseeable losses, reflecting the unpredictable nature of data value and recovery complexity.
4. I think that this looks at data limitations from a more legal standpoint rather than business intelligence standpoint.
It really only talks about data limitations as something that you need to explicitly exclude and state - So in this case, it doesn't really agree with Claude's statement.
In my opinion, the difference in opinion is pretty important, though.
