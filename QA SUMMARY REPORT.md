Here is your QA report properly formatted for a **Markdown (.md) file**:

---

# QA Summary Report

## Game Tested

**Karim Fist Bump**

## Dev Team

* Lucas
* Jack
* Parth
* Biruk

## QA Team

* Karan Modi
* Maxwell Noffsinger
* Sam Taiwo
* Jessica Kamienski

**Testing Period:** Week 6 (Tue–Fri)
**Report Date:** 2/13/2026

---

# Executive Summary

We conducted comprehensive QA testing on **Karim Fist Bump** over 4 days. Our team tested every core feature, ran happy and sad test scenarios, and filed **5 GitHub Issues** documenting bugs across all severity levels.

### Key Finding

The core game loop works, but UI and visuals need bug fixes.

---

# Testing Overview

## What We Tested

* ✅ Normal Gameplay
* ✅ Snake Gameplay
* ✅ Extreme Edge Cases
* ✅ GUI and Visuals
* ✅ Sequences of Events (Fist Bump Event)

---

## Coverage Summary

### Features Tested

| Feature                    | Coverage |
| -------------------------- | -------- |
| Clicking Feature           | 100%     |
| Snake Feature              | 100%     |
| Shop Feature               | 100%     |
| Fist Bump Power-Up Feature | 100%     |

---

## Test Types

* **Functional Testing** – Program works as intended
* **Negative Testing** – Tested failure scenarios (e.g., too many Nayans causing crashes)
* **Exploratory Testing** – Creative scenarios (e.g., reaching infinity and “beating” the game)

---

# Bug Summary

## By Severity

| Severity  | Count |
| --------- | ----- |
| Critical  | 1     |
| High      | 0     |
| Medium    | 2     |
| Low       | 2     |
| **Total** | **5** |

---

## By Category

| Category         | Count |
| ---------------- | ----- |
| Input Validation | 1     |
| Logic Errors     | 1     |
| State Management | 0     |
| UI/UX Issues     | 3     |
| Other            | 0     |

---

# Critical Issues (Must Fix Before Handoff)

These bugs break core gameplay or make the game unplayable.

| # | Title                             | Severity | GitHub Link                                                                                                      |
| - | --------------------------------- | -------- | ---------------------------------------------------------------------------------------------------------------- |
| 1 | Game crashes with too many Nayans | Critical | [https://github.com/Staiwo100/Karim-Clicker-QA/issues/5](https://github.com/Staiwo100/Karim-Clicker-QA/issues/5) |

---

# High-Priority Issues (Fix ASAP)

No high-priority bugs were recorded.

---

# Medium & Low Priority Issues

| # | Title                                              | Severity | GitHub Link                                                                                                      |
| - | -------------------------------------------------- | -------- | ---------------------------------------------------------------------------------------------------------------- |
| 1 | Fist bumps do not disappear after use              | Medium   | [https://github.com/Staiwo100/Karim-Clicker-QA/issues/2](https://github.com/Staiwo100/Karim-Clicker-QA/issues/2) |
| 2 | Unable to buy upgrades when player can afford them | Low      | [https://github.com/Staiwo100/Karim-Clicker-QA/issues/1](https://github.com/Staiwo100/Karim-Clicker-QA/issues/1) |
| 3 | Player can reach Infinity                          | Medium   | [https://github.com/Staiwo100/Karim-Clicker-QA/issues/4](https://github.com/Staiwo100/Karim-Clicker-QA/issues/4) |
| 4 | Nayan Patel covers up UI                           | Low      | [https://github.com/Staiwo100/Karim-Clicker-QA/issues/3](https://github.com/Staiwo100/Karim-Clicker-QA/issues/3) |

---

# Testing Insights

## What Worked Well

* Code quality was up to standard and easy to interpret
* Documentation and commenting made functions easier to understand
* Core clicking mechanic performed as expected without UI bugs

---

## Areas for Improvement

* UI design and formatting
* Number logic errors
* Snake game needs clearer explanation

---

## Patterns Noticed

* Several UI/UX issues
* Asset overload (too many Nayans) causes performance issues
* High object counts lead to crashes and UI instability

---

# Recommendations for Dev Team

## 🔴 Priority 1 – Critical Fixes

* **Fist Bump Power-Up Bug**

  * Power-ups do not disappear
  * Can be reused indefinitely
  * Causes screen clutter

* **Upgrade Purchase Bug**

  * Players cannot buy upgrades when money is earned passively
  * Blocks a key progression mechanic

* **Too Many Nayans Crash**

  * Excessive Nayan count crashes UI
  * Makes game unplayable

---

## 🟠 Priority 2 – Important Fixes

* **Nayan UI Overlap**

  * Nayans cover important UI elements
  * May contribute to crash behavior

---

## 🟢 Priority 3 – Optional / Polish

* Prevent player from reaching Infinity
* Clarify Snake game reward logic

---

# Test Environment

* **Platform:** Browser / VSCode Live Server
* **Game Version:** `4152206139581a955705d9014883dd7fc0300f76`
* **Testing Tools:**

  * Manual Testing
  * GitHub Issues
  * VSCode

---

# GitHub Issues Summary

* **Total Issues:** 5
* **Closed:** 0
* **Open:** 5
* Tag: `qa-week6`

See Dev Team repository for full issue list.

---

# Conclusion

The game has **5 documented issues** ranging from critical to cosmetic.

With focused effort on critical bugs, the core gameplay loop remains playable.
Primary areas needing attention:

* Input validation
* UI/UX stability
* Asset overload handling

---

# QA Team Sign-Off

**Test Lead:** Maxwell Noffsinger
**Submitted:** 2/13/2026

### Team Members

* Samuel Taiwo
* Karan Modi
* Maxwell Noffsinger
* Jessica Kamienski

---

# Appendix: Detailed Test Scenarios

## Scenario 1 – Happy Path

**Result:** Passed

**Notes:**
There is no limit to the number of power-ups you can buy, and there are no levels. The player continues clicking and completing tasks/mini-games indefinitely.

---

## Scenario 2 – Input Validation

**Result:** Partial

**Notes:**
Most inputs work. However, if the player gains only passive income (without clicking), they are unable to purchase upgrades.

---

## Scenario 3 – Edge Cases

**Result:** Partial

**Notes:**

* High integer values convert to “Infinity”
* Around 500–1000 Nayans (depending on PC performance) causes:

  * Major slowdown
  * UI disappearing
  * Eventual crash

---

# Questions for Dev Team

1. Is the Snake game intended to reward money?
2. Is cutting through walls intended behavior?
3. Should the 2x multiplier apply to Snake game rewards?

---

**End of Report**
