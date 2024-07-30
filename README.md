# Recommander-System-WandB
## Report: 
* in train we have 200,000 unique sessions, with varying event lengths.
* in test we have another 200,000 unique sessions (no session in the test set it also in the train set)

Test- there are on average 5 events per session (that are truncated in time, so they were extracted from longer sessions - like these 5 events are subsets of a longer set of events?).

**Scope**: For session 9999 (e.g.) in test set I have 5 events. Use an algorithm (trained on train) + these 5 previous events as guideline to predict for session 9999 up to 20 values for each type of event.