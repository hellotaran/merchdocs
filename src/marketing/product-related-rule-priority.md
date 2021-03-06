---
conditions: Default.EE-B2B
title: Related Product Rule Priority
---

At any given time, there might be a number of active rules that can be triggered to display related products, up-sells, and cross-sells. The priority of each rule determines the order in which the products appear on the page. The value can be set to any whole number, with one having the highest priority.

The number of product IDs that can be included in a product relations rule is determined by the Result Limit value, which has a maximum of twenty. The Result Limit value, combined with the configurable maximum for the specific rule-based product promotion becomes the “real limit,” and determines the actual number of matching products that can appear in the list.

    [Result Limit] + [Configurable Maximum] = [Real Limit]

For example, suppose you have three rules, with a priority of one, two, and three.

* There are two matching products returned for Rule 1, six matching products for Rule 2, and twenty matching products for Rule 3.
* In the configuration, the Maximum Number of Products for Related Products List is set to six.

| Rules | Priority | Matching Products |
|---|---|
| Rule 1 | 1 | 2 |
| Rule 2 | 2 | 6 |
| Rule 3 | 3 | 20 |

If the first rule returns more matching products than allowed by the “configurable maximum limit,” but less than the “real limit,” the matching products from the other existing rules are used—in order of priority—until the “real limit” is reached.

By priority, the matching products returned from Rule 1 can be used first to fill all twenty-six available slots. Because Rule 1 returned only two matching products, there is still room for twenty-four more. Rule 2 has the next highest priority, and returns six more matching products. There are now eighteen available slots to be filled. Rule 3 has the next level of priority, with enough matching products to fill the remaining eighteen slots. When all available slots are filled, and depending on the rotation mode that is set, the list might be shuffled, and then reduced to the “configurable maximum limit”. In this case, the remaining six products appear in the store.
