# Audit: @medxkuber, 2026-11-07

Source: Instagram Graph API lifetime insights via the connected account.
655 followers. 40 posts, 2026-05-18 to 2026-11-06.

Baseline set: 30 reels (2026-05-19 to 2026-10-05). Excluded: 3 trial reels
(2026-05-18), 4 reels posted 2026-11-06 (under 24h old), 3 carousels (n too
small to rank against reels). Median views of the baseline: **3,672**.

Not available from the API: per-post non-follower share, per-reel follows,
retention graph. "Hold" below is 100 minus `reels_skip_rate` (share of viewers
who did not swipe away in the first 3s).

Theme labels were inferred from captions only (I could not see the videos).
"Med Edu" = reels with the "comment notes" CTA or a medical-topic caption.

## Top 5 by outlier multiple

| x | views | reach | hold | avg watch | sends | saves | theme | date |
|---|---|---|---|---|---|---|---|---|
| 4.54 | 16,661 | 12,915 | 46% | 7.7s | 139 | 303 | Med Edu | 06-04 |
| 4.17 | 15,314 | 8,958 | 66% | 7.6s | 64 | 26 | Opinion (cadaver respect) | 06-12 |
| 2.80 | 10,293 | 7,043 | 16% | 3.3s | 13 | 12 | Collab (Neuroflip) | 07-06 |
| 2.65 | 9,731 | 7,545 | 53% | 13.9s | 199 | 328 | Building Prescribed Ep 01 | 08-17 |
| 1.64 | 6,007 | 4,551 | 41% | 7.3s | 30 | 110 | Med Edu | 06-03 |

## Bottom 5

| x | views | hold | avg watch | sends | saves | theme | date |
|---|---|---|---|---|---|---|---|
| 0.74 | 2,699 | 37% | 7.0s | 6 | 11 | Med Edu (occupation) | 06-24 |
| 0.72 | 2,650 | 53% | 10.0s | 17 | 40 | Building Prescribed | 08-18 |
| 0.69 | 2,517 | 44% | 10.0s | 15 | 28 | Opinion (ward learning) | 08-18 |
| 0.58 | 2,118 | 33% | 4.3s | 4 | 8 | Lifestyle (lock-in) | 10-05 |
| 0.57 | 2,091 | 25% | 5.3s | 4 | 8 | Med Edu (LHF breathlessness) | 08-13 |

## By theme (medians)

| theme | n | x | hold | avg watch | sends / 1k reach | saves / 1k reach |
|---|---|---|---|---|---|---|
| Building Prescribed | 2 | 1.69 | 53% | 12.0s | 17.0 | 30.6 |
| Med Edu | 10 | 1.04 | 38% | 6.9s | 6.2 | 13.4 |
| Opinion | 2 | 2.43 | 55% | 8.8s | 7.4 | 8.6 |
| Lifestyle / mood | 13 | 0.95 | 48% | 5.3s | 2.2 | 2.5 |

## Findings

1. **Lifestyle/mood reels get average views and almost nothing else.** 13 of 30
   reels; median 2.2 sends and 2.5 saves per 1k reach, against 6.2 / 13.4 for
   Med Edu and 17 / 31 for Building Prescribed. The account's goal is saves and
   shares, so these are the bottom of the account by the metric that matters.
   Confidence: high (n=13 vs 10).
2. **Building Prescribed Ep 01 is the best reel on the account**, not the one
   with the most views: 26.4 sends and 43.5 saves per 1k reach, 13.9s average
   watch. Both are the highest of all 30. n=1 for that format, so it is a lead,
   not a pattern. Episode 2 was never made.
3. **Med Edu has a hook problem, not a content problem.** Lowest median hold of
   any theme (38%; the LHF reel 25%) but second-highest saves. The people who
   get past second 3 save it. Fix the first 3 seconds, not the topics.
4. **Hold at 3s does not explain the ranking overall** (top 5 avg 44% vs bottom
   5 avg 38%; correlation with outlier multiple 0.24). Theme does.
5. **The Neuroflip collab is not a hit.** 2.8x views, but 16% hold, 3.3s watch,
   1.8 sends per 1k. It was distributed, not watched.
6. **Reach is not the bottleneck, follows are.** Every baseline reel reached
   more accounts than the 655 followers the account has (min 1,516), so at
   least 57% of reach on every reel, and 95% on the top one, was non-followers.
   The reels travel; the profile does not convert. Next: `/ig-profile`.
7. **Cadence collapsed.** 15 reels in June (median 4,406 views), 6 in July, 4 in
   August, 1 each in September and October.
8. **The same diabetes reel was posted 3 times within 7 minutes on 11-06**
   (1,832 / 290 / 192 views), plus an uncaptioned reel that evening. If these
   were not trial reels, they split distribution against each other.

Day of week and time not examined: theme already explains the spread.

## Stop / do more

- STOP: caption-only mood reels (">>>>", "lock-in", "jack of all trades").
- DO MORE: Building Prescribed episodes, and Med Edu with rebuilt hooks.
- NEXT: `/ig-profile` (conversion), then `/ig-plan` from this file.
