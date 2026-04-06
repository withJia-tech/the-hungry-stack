# kitchen-tests — Cucumber

## The exercise
Write a test in plain English. Then make the code pass it.

```gherkin
Feature: The menu knows its dishes

  Scenario: Asking for laksa
    Given the menu exists
    When I ask for "laksa"
    Then I should get a price
```

## The lesson
You wrote a test in language a human can read. Cucumber connected each English sentence to a piece of code (a "step definition"). The test is the spec.

## You'll know it works when
Running cucumber prints a green "1 scenario passed".

## Reflection (fill in after)
What surprised me:
What confused me:
What I want to try next:
