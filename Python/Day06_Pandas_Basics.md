reviews.rename(columns={'points': 'score'})

reviews.rename(index={0: 'firstEntry', 1: 'secondEntry'})
reviews.rename_axis("wines", axis='rows').rename_axis("fields", axis='columns')
