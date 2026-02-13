QA Summary Report 

Game Tested: [Karim Fist bump] 

Dev Team: [Lucas, Jack, Parth, Biruk] 

QA Team: [Karan Modi, Maxwell Noffsinger, Sam Taiwo, Jessica Kamienski] 

Testing Period: Week 6 (Tue–Fri) 

Report Date:  2/13/2026 

Executive Summary 

We conducted comprehensive QA testing on [Karim Fist Bump] for over 4 days. Our team tested [every core feature], ran [happy and sad test scenarios], and filed [3 GitHub Issues] documenting bugs across all severity levels. 

Key Finding: [The core game loop works, but UI and visuals need some bug fixes. 

Testing Overview 

What We Tested 

Normal Gameplay ✓ 

Snake Gameplay ✓ 

Extreme edge cases ✓ 

GUI and visuals ✓ 

Sequences of events (fist bump event) ✓ 

 

Coverage Summary 

Features Tested: [List core features and % coverage] 

Clicking Feature: 100% tested 

Snake Feature: 100% tested 

Shop Feature: 100% tested 

Fist bump powerup Feature 100% tested 

Test Types: [Types of testing we did] 

Functional testing (Program works as intended) 

Negative testing (If there are too many assets on screen, the game will break. For example, if there are too many Nayan's) 

Exploratory testing (We did test creative scenarios. For example, you can reach infinity and “beat” the game. 

Bug Summary 

By Severity 

Critical: 1 bug (game-breaking) 

High: 0 bugs (core features broken) 

Medium: 2 bugs (partial functionality issues) 

Low: 2 bugs (cosmetic or minor edge cases) 

Total Bugs Filed: 5 

By Category 

Input Validation: 1 bug 

Logic Errors: 1 bug 

State Management: 0 bugs 

UI/UX Issues: 3 bugs 

Other: 0 bugs 

Critical Issues (Must Fix Before Handoff) 

These bugs prevent the game from being playable or break core mechanics. 

# 

Title  

Severity 

GitHub Issue Link 

1 

Game Crashes with too many nayans 

Unable to buy upgrades even when the player can afford them 

Paragraph locked by Samuel Taiwo
Critical 

https://github.com/Staiwo100/Karim-Clicker-QA/issues/5 

 

 

 

 

 

 

 

 

High-Priority Issues (Fix ASAP) 

These bugs affect core features but don't prevent gameplay. 

No High-Priority bugs were recorded 

Medium & Low Priority Issues 

Documented in GitHub Issues. These can be deferred or fixed in sequence. 

# 

Title  

Severity 

GitHub Issue Link 

1 

Fists bumps do not disappear after using them 

 

Medium 

https://github.com/Staiwo100/Karim-Clicker-QA/issues/2 

 

2 

Unable to buy upgrades even when the player can afford them 

 

Low 

https://github.com/Staiwo100/Karim-Clicker-QA/issues/1 

 

3 

Player can reach Infinity 

Player can reach Infinity 

Paragraph locked by Samuel Taiwo
Medium 

https://github.com/Staiwo100/Karim-Clicker-QA/issues/4 

 

4 

Nayan Patel's cover up UI 

 

Low 

https://github.com/Staiwo100/Karim-Clicker-QA/issues/3 

 

 

Testing Insights 

What Worked Well 

Code Quality was up to standards and easy for tester interpretation 

Documentation and commenting made functions easier to understand 

Core concept of clicking performed as expected with no UI bugs when clicking on it 

Areas for Improvement 

UI design and formatting  

Numbers have logic errors 

Snake game needs more explanation 

Patterns Noticed 

Several UI/UX issues, many of which are simply but others leading to the game crashing and slowing down 

Recommendations for Dev Team 

Critical Fixes (Priority 1) 

The Fist bump powerup bug — The bug not only causes fist bumps to gather on the screen, but it also makes it so the powerup can be used at any time. 

Players not being able to buy upgrades when they can afford them — This bug prevents people from buying upgrades when they make the money from a passive source. This effects a key feature of the game 

Game crashes with too many nayans — If you reach a certain point in the game it can cause the UI to crash, making the game unplayable 

Important Fixes (Priority 2) 

Nayan Patel’s covering up UI — The nayans are too big and can cover up certain parts of the screen. This could also be why the game crashes after so many nayans. 

Polish/Optional Fixes (Priority 3) 

Player reaching infinity 

Test Environment 

Platform: Browser / VSCODE live server 

Game Version: 4152206139581a955705d9014883dd7fc0300f76 

Testing Tools: Manual testing + GitHub Issues + VSCODE 

All GitHub Issues 

Complete list of filed bugs: See dev team repo for all open GitHub Issues tagged qa-week6 

Total: 5 issues 

Closed: 0 

Open: 5 (for dev team to fix in Week 7) 

Conclusion 

The game has 5 documented issues ranging from critical to cosmetics. With focused effort on critical bugs, the core gameplay loop is playable. Input validation and UI/UX issues are the areas needing the most attention. 

QA Team Sign-Off 

Test Lead: Maxwell Noffsinger 

Submitted: 2/13/26 

Team Members: 

[Samuel Taiwo] 

[Karan Modi] 

[Maxwell Noffsinger] 

[Jessica Kamienski] 

Appendix: Detailed Test Scenarios 

Scenario 1: Happy Path 

Result: Passed 

Notes:  There is no limit to the number of power-ups you can buy, and there are no levels to get through. You just keep clicking and completing the tasks and mini games until you get bored 

Scenario 2: Input Validation 

Result: Partial 

Notes: Most inputs work, but if you don’t click and gain passive income, you are unable to buy upgrades, which is a weird bug. 

Scenario 3: Edge Cases 

Result: Partial 

Notes: Edge cases were tested for integer limits and Nayan’s. Whenever you reach a certain high enough number, the value changes to “infinity”. Whenever the user reaches around 500-1000 Nayan’s (depending on users’ PC), the game begins to crash and slow down. UI begins to bug out and disappears for long periods of time. 

Questions for Dev Team (If Applicable) 

If there were ambiguities in how the game should work, note them here so dev team can clarify in Week 7: 

Is the Snake game supposed to give you money? Also is it intended for you to be able to cut corners and go across the snake map by going through the walls. Also, the 2x multiplier doesn’t work on the snake game winning money. 

End of Report 

 
