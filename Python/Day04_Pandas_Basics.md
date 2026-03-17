reviews.groupby('points').points.count()
reviews.groupby(['country']).price.agg([len, min, max])
countries_reviewed.reset_index()

countries_reviewed.sort_values(by='len') // default to an ascending sort
countries_reviewed.sort_values(by='len', ascending=False)

countries_reviewed.sort_values(by=['country', 'len'])
