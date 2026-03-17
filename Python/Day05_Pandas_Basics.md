reviews.price.dtype

reviews.points.astype('float64')//it's possible to convert a column of one type into another wherever such a conversion makes sense by using the astype() function

reviews[pd.isnull(reviews.country)] // for null value

reviews.region_2.fillna("Unknown") // fill a null value

reviews.taster_twitter_handle.replace("@kerinokeefe", "@kerino") // from kerinokeefe to kerino
