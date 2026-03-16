reviews.points.describe() //This method generates a high-level summary of the attributes of the given column.
reviews.points.mean()
reviews.taster_name.unique() //To see a list of unique values we can use the unique() function
reviews.taster_name.value_counts() //To see a list of unique values and how often they occur in the dataset

review_points_mean = reviews.points.mean()
reviews.points.map(lambda p: p - review_points_mean)

def remean_points(row):
    row.points = row.points - review_points_mean
    return row

reviews.apply(remean_points, axis='columns')

reviews.country + " - " + reviews.region_1
