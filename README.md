[ffuenf-magento-paypal_germany_fix](https://github.com/ffuenf/ffuenf-magento-paypal_germany_fix)
=================

This issue is still not fixed in Magento CommunityEdition 1.6.2.0 and it was first reported back in v1.4.x, well over a year ago.

Orders placed using paypal standard are marked as "Supsected Fraud" upon closing the orders out in PayPal. Line items are passed to paypal and it seems that the calculations within the magento store do not match what is returned from paypal, so the order is marked as fraud.

Current community fixes involve disabling the fraud feature or constantly running cron jobs to change order status levels within the database manually. Neither of these methods is acceptable any longer. We need a code fix from the Magento Team.

Information
-----------

Please use with caution! Currently this temporary fix disables fraud detection manually, so you can at least edit orders in the magento backend. The amounts are still charged with a 1-Cent difference in Paypal.

Bug reports
-----------

+ http://www.magentocommerce.com/boards/viewthread/222075/P60/#t384166
+ http://www.magentocommerce.com/bug-tracking/issue?issue=12685

Authors
-------

**Achim Rosenhagen**

+ http://twitter.com/wuerml
+ http://github.com/wuerml
