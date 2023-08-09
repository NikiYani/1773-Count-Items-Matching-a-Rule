# 1773. Count Items Matching a Rule

You are given an array items, where each items[i] = [typei, colori, namei] </br>
describes the type, color, and name of the ith item. </br>
You are also given a rule represented by two strings, ruleKey and ruleValue. </br>

The ith item is said to match the rule if one of the following is true: </br>

ruleKey == "type" and ruleValue == typei. </br>
ruleKey == "color" and ruleValue == colori. </br>
ruleKey == "name" and ruleValue == namei. </br>
Return the number of items that match the given rule. </br>

## Example 1:

Input: items = [["phone","blue","pixel"],["computer","silver","lenovo"],["phone","gold","iphone"]], ruleKey = "color", ruleValue = "silver" </br>
Output: 1 </br>
Explanation: There is only one item matching the given rule, which is ["computer","silver","lenovo"]. </br>

## Example 2:

Input: items = [["phone","blue","pixel"],["computer","silver","phone"],["phone","gold","iphone"]], ruleKey = "type", ruleValue = "phone" </br>
Output: 2 </br>
Explanation: There are only two items matching the given rule, which are ["phone","blue","pixel"] and ["phone","gold","iphone"]. Note that the item  </br>["computer","silver","phone"] does not match. </br>

## Constraints:

1 <= items.length <= 104 </br>
1 <= typei.length, colori.length, namei.length, ruleValue.length <= 10 </br>
ruleKey is equal to either "type", "color", or "name". </br>
All strings consist only of lowercase letters. </br>
