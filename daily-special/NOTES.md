# daily-special — Redis

## The exercise
Store today's "dish of the day" in Redis. Retrieve it. Change it. Set an expiry. Watch it disappear.

## The lesson
**Expiry.** Redis is a place where things forget themselves on purpose. That's a feature, not a bug.

## Try this
1. `SET dish_of_the_day "laksa"`
2. `GET dish_of_the_day`
3. `SET dish_of_the_day "kaya toast" EX 30`
4. Wait 30 seconds. `GET dish_of_the_day` again. Where did it go?

## Reflection (fill in after)
What surprised me:
What confused me:
What I want to try next:
