# Market Basket Analysis under periodic pattern mining

Market Basket Analysis is one of the key techniques used by large retailers to uncover associations between items. It works by looking for combinations of items that occur together frequently in transactions. To put it another way, it allows retailers to identify relationships between the items that people buy.

We all have been shopping more from online e-commerce sites recently, probably due to the lock-down imposed in most parts of the world. You must have noticed an up-sell feature named ‘frequently bought together’ or ‘other recommendations’ in most of these sites, for instance Amazon where it predicts what all items would go-along with the item that you have just added to the cart. Customers are given the choice of adding all the items shown under this feature to the cart or select the required ones. Amazon does it thorough what they call ‘item-to-item collaborative filtering’ where it runs recommendation algorithms based on the item-search history of the customer to improve the shopping experience. In the case of offline retailers, it works pretty much the same. Let us consider the basic example of Bread and Jam. If the retailer finds that there is an increase in the sales of bread, he/she can further up-sell by giving a discount in the price of jam, so that more customers are bound to buy them together.

This entire process of analyzing the shopping trends of customers is called ‘Market Basket Analysis’. It is an analyzing technique based on the idea that if we buy an item then we are bound to buy or not-buy a group (or single) items. For example, if a customer is buying bread then the chances of him/her buying jam is more. It can be said that between jam and bread an association Rule applied.

Association Rules are widely used to analyze retail basket or transaction data, and are intended to identify strong rules discovered in transaction data using measures of interestingness, based on the concept of strong rules. This can be thought of as an IF-THEN relationship. If bread is bought by a customer then the chances of item jam being bought by the same user in the same transaction is found out. Here bread is called the Antecedent and jam the consequent. Antecedents are primary item that are found in the basket and consequents are the items that are found with an antecedent/group of antecedents.

Periodic Pattern Mining:

Consider a database of transactions depicted below. Each transaction is a set of items (symbols), and transactions are ordered by their time.

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

Here, the database contains seven transactions labeled T1 to T7. This database format can be used to represent all kind of data. However, for our example, assume that it is a database of customer transactions in a retail store. The first transaction represents that a customer has bought the items a and c together. For example, a could mean a bread, and c could mean jam.

Having such a database of objects or transactions, it is possible to find periodic patterns. The concept of periodic patterns is based on the notion of period.

A period is the time elapsed between two occurrences of a pattern.  It can be counted in terms of time, in terms of a number of transactions or something else. Considering the item sets (set of items) {a,c}, this itemset has five periods. 

The first period of {a,c} is what appeared before the first occurrence of {a,c}. By definition, if {a,c} appears in the first transaction of the database, it is assumed that this period has a length of 1.

The second period of {a,c} is the gap between the first and second occurrences of {a,c}. The first occurrence is in transaction T1 and the second occurrence is in transaction T3. Thus, the length of this period is said to be 2 transactions.

The third period of {a,c} is the gap between the second and third occurrences of {a,c}. The second occurrence is in transaction T3 and the third occurrence is in transaction T5. Thus, the length of this period is said to be 2 transactions.

The fourth period of {a,c} is the gap between the third and fourth occurrences of {a,c}. The third occurrence is in transaction T5 and the fourth occurrence is in transaction T6. Thus, the length of this period is said to be 2 transactions.

Now, the fifth period is interesting. It is defined as the time elapsed between the last occurrence of {a,c} (in T6) and the last transaction in the database, which is T7. Thus, the length of this period is also 1 transaction.

Thus, in this example, the list of period lengths of the pattern {a,c} is: 1,2,2,1,1.

Though it seems to be meaningless, let us put it into a context. If I set the maximum period length is 3 to meet the requirement of being periodic, then I can say pattern {a,c} is periodic. If this dataset is for a single e-commercial account and transaction 1 to transaction 7 are limited to every weekends. Then a pattern related to time period can be found by comparing this pattern to other patterns limited in other days.

Periodic mining is a new approach in data mining which has gained its significance these days. This field is evolving due to needs in different applications and limitations of data mining. This would enhance the power of existing data mining techniques. It may be helpful in:
1. find out concealed patterns from large amount of data.
2. Automatically track the changes in facts from previous data
3. Predicting future association rules as well as gives us right methodology to find out outliers.
