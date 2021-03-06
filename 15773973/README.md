[rdar://15773973](rdar://15773973)

## Summary:
When scrolling a tableview of animated images, certain sections of a UITabBar will often appear to be fully transparent instead of blurring the content behind. This is a regression in iOS 7.1. This behavior does not occur in 7.0.x.

## Steps to Reproduce:
(Sample Code Attached)

1. Install Xcode5-Beta3
2. Create a UITabBarController with a UINavigationController in the view controllers array that contains a UITableViewController
3. In the UITableViewController, display a series of animated images.
4. Scroll the table view quickly.

## Expected Results:
The tab bar remains translucent and blurs the content in the tableview.

## Actual Results:
Parts of the tab bar become fully transparent while scrolling.

## Version:
iOS 7.1 beta 3

## Notes:

Configuration:
Occurs on both the iOS Simulator and on iPhone 5s (at least).
