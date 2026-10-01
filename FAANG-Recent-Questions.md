# FAANG / MAANG+ Most Recently Asked Coding Interview Questions

> A comprehensive list of the most recently asked coding interview questions at top tech companies (2025-2026). Questions are organized by company and topic to help you prepare effectively.
>
> **Looking for AI labs?** DeepMind, xAI, Mistral, Perplexity, Scale AI, Cohere, Cursor, Waymo, Sierra, Glean and more live in the companion [AI Labs & AI Companies guide](./AI-Companies-Interview-Questions.md).

> **More from this repo**: [All guides](./README.md) | [AI labs](./AI-Companies-Interview-Questions.md)   | [Blind 75](./Blind-75.md) | [NeetCode 150](./NeetCode-150.md)

## The Single Biggest Change in 2026: AI-Assisted Rounds

The format shifted more in the last year than in the previous five. What changed, and where:

| Company | AI policy in interviews |
| ------- | ----------------------- |
| **Meta** | AI-enabled coding round rolling out to all SWE roles, 3-panel CoderPad, AI reads files but can't edit. For E6+ it *is* the coding round. |
| **Google** | Piloting an AI-assisted "code comprehension" round with Gemini; simultaneously reinstated an in-person round to curb cheating. |
| **LinkedIn** | AI-enabled round is now standard: one of two coding rounds, scored 1-4, where 3 passes. |
| **DoorDash** | Publicly rebuilding interviews around AI: a 60-min AI-assisted working session in your own IDE. |
| **OpenAI** | Agentic coding round in beta (drive an AI agent on a real codebase). The *only* round where AI is allowed. |
| **Anthropic** | Split policy: AI permitted on the performance take-home, strictly prohibited in live interviews. |
| **Sierra** | Removed algorithm interviews entirely. Plan -> Build (2h with any AI) -> Review. |
| **Microsoft** | Team-dependent (CoreAI/Copilot teams may allow GitHub Copilot). Ask your recruiter. |
| **Tesla** | Googling allowed; LLM use at interviewer discretion. |
| **Amazon, Apple, ByteDance, Palantir, Uber, Airbnb** | No AI-assisted round reported; ByteDance and Palantir explicitly ban AI use. |

Where AI is allowed, the rubric moved to **verification**: test before you trust, and explain the output. Where it's banned, expect proctoring, in-person rounds, and debug-the-supplied-code formats instead.

## Table of Contents

- [Meta (formerly Facebook)](#meta-formerly-facebook)
  - [Arrays and Strings](#meta-arrays-and-strings)
  - [Linked Lists](#meta-linked-lists)
  - [Trees and Graphs](#meta-trees-and-graphs)
  - [Recursion and Backtracking](#meta-recursion-and-backtracking)
  - [Sorting and Searching](#meta-sorting-and-searching)
  - [Dynamic Programming](#meta-dynamic-programming)
  - [Design](#meta-design)
- [Amazon](#amazon)
  - [Arrays and Strings](#amazon-arrays-and-strings)
  - [Sliding Window and Two Pointers](#amazon-sliding-window-and-two-pointers)
  - [Trees and Graphs](#amazon-trees-and-graphs)
  - [Heaps and Priority Queues](#amazon-heaps-and-priority-queues)
  - [Dynamic Programming](#amazon-dynamic-programming)
  - [Design](#amazon-design)
- [Apple](#apple)
  - [Arrays and Strings](#apple-arrays-and-strings)
  - [Trees and Graphs](#apple-trees-and-graphs)
  - [Design and System Coding](#apple-design-and-system-coding)
- [Netflix](#netflix)
  - [System Design Coding](#netflix-system-design-coding)
  - [Algorithms](#netflix-algorithms)
- [Google](#google)
  - [Arrays and Strings](#google-arrays-and-strings)
  - [Trees and Graphs](#google-trees-and-graphs)
  - [Dynamic Programming](#google-dynamic-programming)
  - [Binary Search and Special Topics](#google-binary-search-and-special-topics)
- [Microsoft](#microsoft)
  - [Arrays and Strings](#microsoft-arrays-and-strings)
  - [Linked Lists](#microsoft-linked-lists)
  - [Trees and Graphs](#microsoft-trees-and-graphs)
  - [Design and Hard Problems](#microsoft-design-and-hard-problems)
- [LinkedIn](#linkedin)
  - [Data Structure Design](#linkedin-data-structure-design)
  - [Trees and Graphs](#linkedin-trees-and-graphs)
  - [Arrays and DP](#linkedin-arrays-and-dp)
- [OpenAI](#openai)
  - [Core Custom Problems](#openai-core-custom-problems)
  - [LeetCode-Equivalent Problems](#openai-leetcode-equivalent-problems)
  - [System Design](#openai-system-design)
  - [ML and AI Technical](#openai-ml-and-ai-technical)
- [Anthropic](#anthropic)
  - [Core Custom Coding Problems](#anthropic-core-custom-coding-problems)
  - [LeetCode Practice](#anthropic-leetcode-practice-mapped-to-focus-areas)
  - [System Design](#anthropic-system-design)
  - [ML and AI Safety](#anthropic-ml-and-ai-safety)
- [Palantir](#palantir)
  - [Coding Problems](#palantir-coding-problems)
  - [OA Problems](#palantir-oa-problems-2026-hackerrank-3-part)
  - [System Design](#palantir-system-design)
  - [Unique Rounds](#palantir-unique-rounds)
- [Tesla](#tesla)
  - [Algorithms](#tesla-algorithms)
  - [System Design](#tesla-system-design)
  - [Embedded Systems](#tesla-embedded-systems)
- [Databricks](#databricks)
  - [Algorithms and Design](#databricks-algorithms-and-design)
  - [Custom Problems](#databricks-custom-problems)
  - [Concurrency (Dedicated Round)](#databricks-concurrency-dedicated-round)
  - [System Design](#databricks-system-design)
- [Stripe](#stripe)
  - [Coding and Integration](#stripe-coding-and-integration)
  - [Bug Squash and API Design](#stripe-bug-squash-and-api-design)
- [NVIDIA](#nvidia)
  - [Algorithms](#nvidia-algorithms)
  - [GPU and Systems](#nvidia-gpu-and-systems)
- [Uber](#uber)
  - [Algorithms](#uber-algorithms)
  - [System Design](#uber-system-design)
- [ByteDance / TikTok](#bytedance--tiktok)
  - [Algorithms](#bytedance-algorithms)
  - [System Design](#bytedance-system-design)
- [Airbnb](#airbnb)
  - [Algorithms](#airbnb-algorithms)
  - [System Design](#airbnb-system-design)
- [DoorDash](#doordash)
  - [Algorithms](#doordash-algorithms)
  - [AI-Assisted and Custom Rounds](#doordash-ai-assisted-and-custom-rounds)
- [Anduril](#anduril)
  - [Custom Problems](#anduril-custom-problems)
  - [LeetCode Practice](#anduril-leetcode-practice-mapped-to-reported-topics)
  - [System Design](#anduril-system-design)
- [Figma](#figma)
  - [Coding Problems](#figma-coding-problems)
  - [LeetCode Practice](#figma-leetcode-practice-mapped-to-reported-topics)
  - [System Design](#figma-system-design)
  - [Frontend Deep Dive](#figma-frontend-deep-dive-frontend-roles)
- [Ramp](#ramp)
  - [Coding Problems](#ramp-coding-problems)
  - [LeetCode Practice](#ramp-leetcode-practice-mapped-to-reported-topics)
  - [System Design](#ramp-system-design)
- [AI Labs & AI Companies](./AI-Companies-Interview-Questions.md), separate guide: DeepMind, xAI, Mistral, Perplexity, Scale AI, Cohere, Cursor, Waymo, and 10+ more
- [Topic-wise Questions](#topic-wise-questions)

---

## Meta (formerly Facebook)

> **2025-2026 Trends**: De-emphasis of DP, rise of expression parsing/stack problems, streaming and sparse data, speed and clean code prioritized over brute force. ~26% Easy, 60% Medium, 14% Hard. **New in 2026**: AI-Enabled Coding Round rolling out to all SWE roles, 60 min in a 3-panel CoderPad (file explorer, editor, AI chat; GPT-5, Claude Sonnet, Gemini, Llama 4 available; AI reads files but cannot edit). Three phases: (1) fix a non-algorithmic bug, (2) build a 120+ line feature with AI expected, (3) optimize for larger datasets. Scored on problem solving, code quality, **verification of AI output**, and communication, for E4-E5 it randomly replaces one of the two coding rounds; at E6 it also replaces one of two, so a traditional CoderPad round normally remains. Rollout now covers SWE and EM roles up through E7/M2. Candidates report the in-interview AI is weaker than in practice mode. Behavioral round weight increased, it can single-handedly downlevel E5 to E4. Candidates increasingly get *variants* of tagged problems rather than the originals. Two problems in 35 minutes for traditional rounds -- speed is king.

### Meta Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Minimum Remove to Make Valid Parentheses](https://leetcode.com/problems/minimum-remove-to-make-valid-parentheses) | Medium |
| 2 | [Valid Palindrome II](https://leetcode.com/problems/valid-palindrome-ii) | Easy |
| 3 | [Valid Palindrome](https://leetcode.com/problems/valid-palindrome) | Easy |
| 4 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium |
| 5 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 6 | [Move Zeroes](https://leetcode.com/problems/move-zeroes) | Easy |
| 7 | [Add Strings](https://leetcode.com/problems/add-strings) | Easy |
| 8 | [Maximum Swap](https://leetcode.com/problems/maximum-swap) | Medium |
| 9 | [Valid Word Abbreviation](https://leetcode.com/problems/valid-word-abbreviation) | Easy ||
| 10 | [Diagonal Traverse](https://leetcode.com/problems/diagonal-traverse) | Medium |
| 11 | [Next Permutation](https://leetcode.com/problems/next-permutation) | Medium |
| 12 | [Interval List Intersections](https://leetcode.com/problems/interval-list-intersections) | Medium |
| 13 | [Validate IP Address](https://leetcode.com/problems/validate-ip-address) | Medium |
| 14 | [Remove All Adjacent Duplicates in String II](https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string-ii) | Medium |
| 15 | [Greatest Common Divisor of Strings](https://leetcode.com/problems/greatest-common-divisor-of-strings) | Easy |
| 16 | [Toeplitz Matrix](https://leetcode.com/problems/toeplitz-matrix) | Easy |
| 17 | [Find the Length of the Longest Common Prefix](https://leetcode.com/problems/find-the-length-of-the-longest-common-prefix) | Medium |
| 18 | [Longest Substring with At Most K Distinct Characters](https://leetcode.com/problems/longest-substring-with-at-most-k-distinct-characters) | Medium |


### Meta Linked Lists

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists) | Easy |
| 2 | [Copy List with Random Pointer](https://leetcode.com/problems/copy-list-with-random-pointer) | Medium |
| 3 | [Reorder List](https://leetcode.com/problems/reorder-list) | Medium |
| 4 | [Insert into a Sorted Circular Linked List](https://leetcode.com/problems/insert-into-a-sorted-circular-linked-list) | Medium |
| 5 | [Remove Nth Node From End of List](https://leetcode.com/problems/remove-nth-node-from-end-of-list) | Medium |

### Meta Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Binary Tree Vertical Order Traversal](https://leetcode.com/problems/binary-tree-vertical-order-traversal) | Medium |
| 2 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium |
| 3 | [Binary Tree Right Side View](https://leetcode.com/problems/binary-tree-right-side-view) | Medium |
| 4 | [Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree) | Easy |
| 5 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium |
| 6 | [All Nodes Distance K in Binary Tree](https://leetcode.com/problems/all-nodes-distance-k-in-binary-tree) | Medium |
| 7 | [Sum Root to Leaf Numbers](https://leetcode.com/problems/sum-root-to-leaf-numbers) | Medium |
| 8| [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 9 | [Shortest Path in Binary Matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix) | Medium |
| 10 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium |
| 11 | [Max Area of Island](https://leetcode.com/problems/max-area-of-island) | Medium |


### Meta Recursion and Backtracking

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number) | Medium |
| 2 | [Permutations](https://leetcode.com/problems/permutations) | Medium |
| 3 | [Subsets](https://leetcode.com/problems/subsets) | Medium |
| 4 | [Remove Invalid Parentheses](https://leetcode.com/problems/remove-invalid-parentheses) | Hard |
| 6 | [Strobogrammatic Number II](https://leetcode.com/problems/strobogrammatic-number-ii) | Medium |

### Meta Sorting and Searching

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Random Pick with Weight](https://leetcode.com/problems/random-pick-with-weight) | Medium |
| 2 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium |
| 3 | [Find Peak Element](https://leetcode.com/problems/find-peak-element) | Medium |
| 4 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 5 | [Pow(x, n)](https://leetcode.com/problems/powx-n) | Medium |
| 6 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium |

### Meta Dynamic Programming

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy |
| 2 | [Word Break](https://leetcode.com/problems/word-break) | Medium |
| 3 | [Decode Ways](https://leetcode.com/problems/decode-ways) | Medium |
| 4 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium |

## Amazon

> **2025-2026 Trends**: Practical, real-world framing. Heap-based reasoning emphasized. OA structure: Q1 is Array/String/Sliding Window, Q2 is Graph/Trees/DP/Heap. ~19% Easy, 60% Medium, 21% Hard. **New in 2026**: HackerRank OA = 2 coding problems (~70 min) + Work Simulation (~20 min) + Work Style Assessment (~10-20 min); the SDE II OA adds a 20-minute System Design scenario section. ~75-80% of OA problems are Medium, wrapped in Amazon-themed framing (servers, warehouses, parcels). Onsite is ~50/50 coding vs Leadership Principles in every round, plus Bar Raiser. Rising: weighted-shortest-path/Dijkstra problems; system design now probes deployment topology and on-call readiness. **No AI-assisted round reported**: Amazon instead rotates custom OA problem sets aggressively, so pattern prep beats memorization. Under-prepared LPs to watch: "Have Backbone, Disagree & Commit", "Are Right A Lot", "Frugality".

### Amazon Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 2 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 3 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium |
| 4 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 5 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium |
| 7 | [3Sum](https://leetcode.com/problems/3sum) | Medium |
| 8 | [Subarray Sum Equals K](https://leetcode.com/problems/subarray-sum-equals-k) | Medium |
| 9 | [Maximum Frequency After Subarray Operation](https://leetcode.com/problems/maximum-frequency-after-subarray-operation) | Medium |
| 10 | [Max Difference You Can Get From Changing an Integer](https://leetcode.com/problems/max-difference-you-can-get-from-changing-an-integer) | Medium |
| 11 | [Analyze User Website Visit Pattern](https://leetcode.com/problems/analyze-user-website-visit-pattern) | Medium |
| 12 | [Find First and Last Position of Element in Sorted Array](https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array) | Medium |

### Amazon Sliding Window and Two Pointers

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium |
| 2 | [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring) | Hard |
| 3 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium |
| 4 | [Longest Repeating Character Replacement](https://leetcode.com/problems/longest-repeating-character-replacement) | Medium |
| 5 | [Sliding Window Maximum](https://leetcode.com/problems/sliding-window-maximum) | Hard |

### Amazon Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 2 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium |
| 3 | [Rotting Oranges](https://leetcode.com/problems/rotting-oranges) | Medium |
| 4 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium |
| 5 | [Binary Tree Zigzag Level Order Traversal](https://leetcode.com/problems/binary-tree-zigzag-level-order-traversal) | Medium |
| 6 | [Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree) | Easy |
| 7 | [Word Search](https://leetcode.com/problems/word-search) | Medium |

### Amazon Heaps and Priority Queues

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium |
| 2 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium |
| 3 | [Task Scheduler](https://leetcode.com/problems/task-scheduler) | Medium |
| 4 | [Maximize Y-Sum by Picking a Triplet of Distinct X-Values](https://leetcode.com/problems/maximize-ysum-by-picking-a-triplet-of-distinct-xvalues) | Medium |
| 5 | [Minimum Cost to Connect Sticks](https://leetcode.com/problems/minimum-cost-to-connect-sticks) | Medium |

### Amazon Dynamic Programming

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium |
| 2 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium |
| 3 | [Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray) | Medium |
| 4 | [Jump Game](https://leetcode.com/problems/jump-game) | Medium |
| 5 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy |
| 6 | [Decode Ways](https://leetcode.com/problems/decode-ways) | Medium |
| 7 | [Word Break](https://leetcode.com/problems/word-break) | Medium |

## Apple

> **2025-2026 Trends**: Practical/applied problems over pure algo puzzles, real Apple workload framing (file dedup, iOS task simulation, API throttling). Stricter expectations on edge cases and memory behavior. Design-oriented coding (LRU Cache is most frequently reported). **Still radically team-dependent. No unified loop**: some teams ask standard LC mediums, embedded/hardware teams ask C/C++ memory/optimization, services teams ask API design or debug-broken-code, some skip LeetCode entirely for architecture or take-homes. **New in 2026**: design-style coding questions are disproportionately common (Time Based KV Store, Design Hit Counter, BST iterators); loops for experienced hires are getting longer, 8-9 rounds over several weeks reported; ICT4 candidates report up to 3 phone screens before onsite. **No AI-assisted rounds reported** as of mid-2026. All experiences describe human-only interviews graded on correctness, memory behavior, and boundary handling rather than Hards.

### Apple Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 2 | [3Sum](https://leetcode.com/problems/3sum) | Medium |
| 3 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 4 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) | Easy |
| 5 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 6 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium |
| 7 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium |
| 8 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock) | Easy |
| 9 | [Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array) | Medium |
| 10 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium |
| 11 | [Permutations](https://leetcode.com/problems/permutations) | Medium |

### Apple Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 2 | [Lowest Common Ancestor of a Binary Tree](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree) | Medium |
| 3 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium |
| 4 | [Sum Root to Leaf Numbers](https://leetcode.com/problems/sum-root-to-leaf-numbers) | Medium ||
| 5 | [Flood Fill](https://leetcode.com/problems/flood-fill) (both BFS and DFS required) | Easy |
| 6 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium |
| 7 | [Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence) | Medium |
| 8 | [House Robber](https://leetcode.com/problems/house-robber) (circular II extension probed) | Medium |

## Netflix

> **2025-2026 Trends**: Streaming/recommendation-themed problem wrappers. Graph-heavy focus (topological sort, shortest path, CDN routing). System design is the pass/fail determinant. Concurrency and rate limiting emphasized. Code must compile and run with unit tests. **Biggest 2026 change: formal engineering levels.** Netflix moved away from the single "Senior Engineer" rung to an explicit multi-band ladder (roughly E1/L4-E7). The same coding answer is now scored against the target level, so an answer that passes at E4 can fail at E6 for being "too tactical." Loops are decentralized and team-owned: hiring manager is involved from the first screen; 4-6 rounds; tech screen is 45 min on CodeSignal or 60 min on CoderPad depending on team; 1-2 directors often sit in onsites. Coding style favors practical mediums over puzzles, streaming aggregation, rate limiting, caching/TTL behavior, parsing, concurrency, frequently re-skinned with Netflix domain (shows, playlists, watch history). The culture/Keeper Test round remains mandatory in every loop.

### Netflix System Design Coding

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 2 | [Design Hit Counter](https://leetcode.com/problems/design-hit-counter) | Medium |
| 3 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium |
| 4 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium |
| 5 | [Logger Rate Limiter](https://leetcode.com/problems/logger-rate-limiter) | Easy |
| 6 | [Min Stack](https://leetcode.com/problems/min-stack) | Medium |

### Netflix Algorithms

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 2 | [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii) | Medium |
| 3 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium |
| 4 | [Network Delay Time](https://leetcode.com/problems/network-delay-time) | Medium |
| 5 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium |
| 6 | [Daily Temperatures](https://leetcode.com/problems/daily-temperatures) | Medium |
| 7 | [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas) | Medium |
| 8 | [Parallel Courses](https://leetcode.com/problems/parallel-courses) | Medium |
| 9 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium |
| 10 | [Course Schedule](https://leetcode.com/problems/course-schedule) | Medium |
| 11 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 12 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium |


## Google

> **2025-2026 Trends**: Graphs appear in 76% of onsite loops at L4+. Sliding window and binary search on answer are top-tier patterns. Trie and Union-Find questions rising. Roughly 19% of reported problems are Hard. Follow-up questions are standard. **New in 2026**: AI-assisted "Code Comprehension" round piloting. Candidates read, debug, and optimize an existing codebase with **Gemini available** in a CoderPad-style environment (file explorer + editor + AI chat); interviewers explicitly score "AI fluency": prompt engineering, output validation, and debugging of AI output. Pilot targets junior/mid-level roles on select US teams; full transition expected within 12-18 months (context: Pichai's April 2026 statement that 75% of new Google code is AI-generated). **In-person round reinstated** for technical hires to combat AI-assisted cheating. Google Hiring Assessment (GHA) mandatory before the phone screen. The Googleyness & Leadership round is now part-technical. A design conversation about a real system you built, defended under scrutiny. **Third change, early-career only**: one traditional technical round is replaced by an open-ended engineering problem session, closer to a discussion of approach than a single correct answer. Reports emphasize deliberately ambiguous problem framing (you must derive the problem structure) and strict production-ready-code grading at L4. No system design round below L5.

### Google Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 2 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium |
| 3 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium |
| 4 | [3Sum](https://leetcode.com/problems/3sum) | Medium |
| 5 | [Group Anagrams](https://leetcode.com/problems/group-anagrams) | Medium |
| 6 | [Product of Array Except Self](https://leetcode.com/problems/product-of-array-except-self) | Medium |
| 7 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 8 | [Find And Replace in String](https://leetcode.com/problems/find-and-replace-in-string) | Medium |
| 9 | [Detect Squares](https://leetcode.com/problems/detect-squares) | Medium |
| 10 | [Pour Water](https://leetcode.com/problems/pour-water) | Medium |
| 11 | [Decode String](https://leetcode.com/problems/decode-string) | Medium |

### Google Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 2 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium |
| 3 | [Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree) | Medium |
| 4 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium |
| 5 | [Accounts Merge](https://leetcode.com/problems/accounts-merge) | Medium |
| 6 | [Evaluate Division](https://leetcode.com/problems/evaluate-division) | Medium |
| 7 | [The Earliest Moment When Everyone Become Friends](https://leetcode.com/problems/the-earliest-moment-when-everyone-become-friends) | Medium 
| 8 | [Step-By-Step Directions From a Binary Tree Node to Another](https://leetcode.com/problems/step-by-step-directions-from-a-binary-tree-node-to-another) | Medium |
| 9 | [Path With Minimum Effort](https://leetcode.com/problems/path-with-minimum-effort) | Medium |
| 10 | [Find Leaves of Binary Tree](https://leetcode.com/problems/find-leaves-of-binary-tree) | Medium |
| 11 | [Longest Word in Dictionary](https://leetcode.com/problems/longest-word-in-dictionary) | Medium |

### Google Dynamic Programming

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Coin Change](https://leetcode.com/problems/coin-change) | Medium |
| 2 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium |
| 3 | [Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence) | Medium |
| 4 | [Longest Arithmetic Subsequence of Given Difference](https://leetcode.com/problems/longest-arithmetic-subsequence-of-given-difference) | Medium |
| 5 | [Maximum Number of Points with Cost](https://leetcode.com/problems/maximum-number-of-points-with-cost) | Medium |
| 6 | [Count Square Submatrices with All Ones](https://leetcode.com/problems/count-square-submatrices-with-all-ones) | Medium |

### Google Binary Search and Special Topics

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium |
| 2 | [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas) | Medium |
| 3 | [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree) | Medium |
| 4 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium |
| 5 | [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array) | Medium |
| 6 | [Task Scheduler](https://leetcode.com/problems/task-scheduler) | Medium |
| 7 | [Range Sum Query - Mutable](https://leetcode.com/problems/range-sum-query-mutable) | Medium |

Segment tree / BIT problems are a Google-distinctive category rarely seen at other FAANG companies.

## Microsoft

> **2025-2026 Trends**: Depth over speed. Higher proportion of backtracking and linked list problems (~29% linked lists). Design-heavy follow-ups standard. **New in 2026**: Process is stable but compressed. Codility/HackerRank-style OA (2 mediums) then 4 virtual onsite rounds usually on a single day; SDE2 loops = 2-3 DSA rounds + LLD + HLD + hiring-manager round. The **"As Appropriate" (AA) round** is formalized, run by Principal EMs, routing candidates into gap-probe / behavioral deep-dive / sell-Microsoft modes; ~85% of candidates reaching AA get offers, but it retains veto power. Behavioral "growth mindset" scoring is now level-banded (L60-62 vs L63-64 vs L65+). **AI-assisted coding rounds are org-specific, not universal**: mostly CoreAI/Copilot-adjacent teams, where you get a dev environment with GitHub Copilot and are evaluated on whether you validate suggestions, keep code readable, and debug incomplete AI output. Ask your recruiter whether your loop includes it. Post-2025 layoffs: junior SDE openings compressed; AI Engineer (Foundry), M365 Copilot Developer, and Azure Architect tracks expanded, adding ML fundamentals, RAG/grounding, multi-agent orchestration, and responsible-AI scenarios.

### Microsoft Arrays and Strings

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Two Sum](https://leetcode.com/problems/two-sum) | Easy |
| 2 | [Merge Sorted Array](https://leetcode.com/problems/merge-sorted-array) | Easy |
| 3 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium |
| 4 | [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters) | Medium |
| 5 | [Set Matrix Zeroes](https://leetcode.com/problems/set-matrix-zeroes) | Medium |
| 6 | [Rotate Image](https://leetcode.com/problems/rotate-image) | Medium |
| 7 | [Sort Colors](https://leetcode.com/problems/sort-colors) | Medium |
| 8 | [Permutation in String](https://leetcode.com/problems/permutation-in-string) | Medium |
| 9 | [Container With Most Water](https://leetcode.com/problems/container-with-most-water) | Medium |
| 10 | [Longest Palindromic Substring](https://leetcode.com/problems/longest-palindromic-substring) | Medium |
| 11 | [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array) | Medium |
| 12 | [3Sum](https://leetcode.com/problems/3sum) | Medium |

### Microsoft Linked Lists

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Add Two Numbers](https://leetcode.com/problems/add-two-numbers) | Medium |
| 2 | [Merge Two Sorted Lists](https://leetcode.com/problems/merge-two-sorted-lists) | Easy |
| 3 | [Copy List with Random Pointer](https://leetcode.com/problems/copy-list-with-random-pointer) | Medium |

### Microsoft Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Number of Islands](https://leetcode.com/problems/number-of-islands) | Medium |
| 2 | [Binary Tree Level Order Traversal](https://leetcode.com/problems/binary-tree-level-order-traversal) | Medium |
| 3 | [Clone Graph](https://leetcode.com/problems/clone-graph) | Medium |
| 4 | [Symmetric Tree](https://leetcode.com/problems/symmetric-tree) | Easy |
| 5 | [Cheapest Flights Within K Stops](https://leetcode.com/problems/cheapest-flights-within-k-stops) | Medium |
| 6 | [Construct Binary Tree from Preorder and Inorder Traversal](https://leetcode.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal) | Medium |
| 7 | [Generate Parentheses](https://leetcode.com/problems/generate-parentheses) | Medium |
| 8 | [Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number) | Medium |

 ## LinkedIn

> **2025-2026 Trends**: The **AI-enabled coding interview is now part of the standard SWE loop**: one of the two coding rounds is replaced by an AI-assisted round on CoderPad with an AI chat panel (choice of models, typically Claude/Opus tiers). The AI **cannot edit code directly**: you paste and verify. Graded on a **4-point scale where 3 passes**, relative to other candidates; interviewers score whether you direct and verify the AI (prompt -> review -> run -> confirm), not whether you can avoid it. **Follow-ups are the real bar**: after working code, questioning pivots to concurrency/thread safety (most common), scaling behavior, malformed input, and production readiness. That's where candidates struggle. Loop: screening (often LC medium + SQL for some roles) -> onsite of 2 coding (1 AI-enabled) + system design + "craftsmanship" (code quality/engineering practices) + hiring manager. Staff loops: 3 DSA (up to LC Hard) + 2 system design + managerial. LinkedIn's classic tagged set still dominates, now wrapped with AI-era production follow-ups.


### LinkedIn Trees and Graphs

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Find Leaves of Binary Tree](https://leetcode.com/problems/find-leaves-of-binary-tree) | Medium |
| 2 | [Find the Celebrity](https://leetcode.com/problems/find-the-celebrity) | Medium |
| 3 | [Lowest Common Ancestor of a BST](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree) | Medium |
| 4 | [Generate Random Point in a Circle](https://leetcode.com/problems/generate-random-point-in-a-circle) | Medium |
| 5 | [Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number) | Medium |

### LinkedIn Arrays and DP

| No. | Question | Difficulty |
| --- | -------- | ---------- |
| 1 | [Can Place Flowers](https://leetcode.com/problems/can-place-flowers) | Easy |
| 2 | [Maximum Subarray](https://leetcode.com/problems/maximum-subarray) | Medium |
| 3 | [Maximum Product Subarray](https://leetcode.com/problems/maximum-product-subarray) | Medium |
| 4 | [Edit Distance](https://leetcode.com/problems/edit-distance) | Medium |
| 5 | [Decode Ways](https://leetcode.com/problems/decode-ways) | Medium |
| 6 | [House Robber II](https://leetcode.com/problems/house-robber-ii) | Medium |
| 7 | [Merge Intervals](https://leetcode.com/problems/merge-intervals) | Medium |
| 8 | [Max Consecutive Ones III](https://leetcode.com/problems/max-consecutive-ones-iii) | Medium |
| 9 | [Valid Perfect Square](https://leetcode.com/problems/valid-perfect-square) | Easy |
| 10 | [Valid Parentheses](https://leetcode.com/problems/valid-parentheses) | Easy |

## OpenAI

> **2025-2026 Trends**: Production over puzzles. Problems drawn from a fixed bank of ~8 core challenges with progressive difficulty layers, and the bank churns (Dependency Version Finder is a new entrant). Python strongly recommended. Coding bar is non-negotiable. Interviewers expect you to "fly through" problems, candidates report typing the whole 60 minutes. **New in 2026**: (1) **Agentic coding round (beta)**: you get an existing codebase and must add features scoped "too large and complex to tackle by hand," so you are *expected* to drive an AI coding agent. This is the **only live round** where AI use is permitted, every other interview strictly prohibits it. (The take-home is the one other carve-out, and only for Applied AI roles; see below.) Not all candidates get it while in beta. (2) The 48-hour take-home is now widely reported as a **paid work trial (~$1,000)** under NDA, scoped for ~3-6 hours of work and graded like a senior engineer's PR review, **"missing test coverage" is the single most-cited rejection reason**, and a design doc explaining tradeoffs is expected. AI tooling is allowed for Applied AI roles, restricted for Core Infra/Research. (3) Official candidate guide published: final loop is 4-6 hours with 4-6 people over 1-2 days; engineering criteria are explicitly "well-designed solutions, high-quality code, optimal performance, good test coverage." Loop = 2 coding + 1 system design + behavioral + hiring manager, plus a 45-min project presentation round (deep defense of a personal project). System design interviewers push 10x/100x/1000x scaling, fault tolerance, and idempotency.


**Progressive layers reported in 2026**: *Resumable Iterator* now runs up to 6 parts (lists -> multi-file with empty files -> async/coroutines -> 2D -> 3D iterators). *CD Directory Navigation* adds `~` home-dir handling and symlink resolution with cycle detection. *GPU Credit Allocation* uses half-open intervals `[start, expiration)`, consumes soonest-expiring first (heap/queue), and must answer balance queries at an arbitrary timestamp.

### OpenAI LeetCode-Equivalent Problems

| No. | Question | Difficulty | Context |
| --- | -------- | ---------- | ------- |
| 1 | [LRU Cache](https://leetcode.com/problems/lru-cache) | Medium | Inference KV cache -- most frequently reported |
| 2 | [Time Based Key-Value Store](https://leetcode.com/problems/time-based-key-value-store) | Medium | Model checkpoint storage |
| 3 | [Snapshot Array](https://leetcode.com/problems/snapshot-array) | Medium | Model state checkpointing |
| 4 | [Web Crawler Multithreaded](https://leetcode.com/problems/web-crawler-multithreaded) | Medium | Training data crawling |
| 5 | [Design Memory Allocator](https://leetcode.com/problems/design-memory-allocator) | Medium | GPU memory management |
| 6 | [Game of Life](https://leetcode.com/problems/game-of-life) | Medium | Extended to infinite board |
| 7 | [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii) | Medium | Interval scheduling |
| 8 | [Encode and Decode Strings](https://leetcode.com/problems/encode-and-decode-strings) | Medium | Serialization family |
| 9 | [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree) | Hard | Data persistence |
| 10 | [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements) | Medium | ML preprocessing |
| 11 | [Course Schedule II](https://leetcode.com/problems/course-schedule-ii) | Medium | Dependency resolution |
| 12 | [Decode String](https://leetcode.com/problems/decode-string) | Medium | String processing |
