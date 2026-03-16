data: 10/24/2025
1. reviews
2. reviews.
3. reviews[''][index]
4. index-based selection: selecting data based on its numerical position in the data. iloc follows this paradigm.(row first, column second)
5. data.iloc[0]  get the first row
6. to get a column, write data.iloc[:, 0]
7. reviews.iloc[:3, 0] range of 0,1,2
8. reviews.iloc[1:3, 0] range of 1,2
9. reviews.iloc[[0, 1, 2], 0]
10. reviews.iloc[-5:] Finally, it's worth knowing that negative numbers can be used in selection. This will start counting forwards from the end of the values.
12. label-based selection：reviews.loc[0, 'country']
                           reviews.loc[:, ['taster_name', 'taster_twitter_handle', 'points']] （loc is inclusive）
13. reviews.set_index("title") manipulate the index
14. reviews.country == 'Italy' condition selection
15. reviews.loc[reviews.country == 'Italy'] choose all with country equals to Italy
16. reviews.loc[(reviews.country == 'Italy') & (reviews.points >= 90)]
17. reviews.loc[(reviews.country == 'Italy') | (reviews.points >= 90)]
18. reviews.loc[reviews.country.isin(['Italy', 'France'])] The first is isin. isin is lets you select data whose value "is in" a list of values. For example, here's how we can use it to select wines only from Italy or France:
19. reviews.loc[reviews.price.notnull()] The second is isnull (and its companion notnull). These methods let you highlight values which are (or are not) empty (NaN)
20. reviews['critic'] = 'everyone' (assign value)
21. reviews['index_backwards'] = range(len(reviews), 0, -1) an iterable of values
