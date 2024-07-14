---
layout: post
title: "Group Testing for Covid-19"
date: 2020-05-12
categories: personalPosts
---

Suppose we need to test 100 people for coronavirus. Say each test takes 5 minutes; so a single machine can do it in 8 hours and 20 minutes. We can reduce that to 5 hours using basic group testing. Suppose for technological reasons we are limited to mixing only 2 samples at a time. Because…

Suppose we need to test 100 people for coronavirus. Say each test takes 5 minutes; so a single machine can do it in 8 hours and 20 minutes. We can reduce that to 5 hours using basic group testing.

Suppose for technological reasons we are limited to mixing only 2 samples at a time. Because of operational reasons, suppose we can take at most 2 samples from each person. Further suppose among all the people who are tested 5% of them are positive (positivity can go higher in severely hit areas).

For each pair of patients, we mix their samples. If the mixture tests negative, they are both clear. If it comes back positive, we test one of them. If he is negative, the other must be positive. If he is positive, we have to test the other person anyway. So either it takes 1 test or at most 3 tests for 2 people.

Now consider 100 people paired into 50 pairs. At 5% positivity rate, we expect at most 5 positive pairs. Therefore at least 45 of the pairs only need 1 test. The other 5 pairs need at most 15 tests. In total only 60 tests are needed. At 5 minutes for each test, that is 5 hours.

If we can take more samples per person and mix samples of more people together, we can achieve higher testing speeds.