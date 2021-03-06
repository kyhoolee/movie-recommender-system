# Movie Recommender System

```html
Version: Spark – 2.2.1, Python – 2.7
```

Command to run on terminal:

```html
spark-submit [CF python file] [input file] [testing file]
```

The above command will generate an `output file` in the current directory 

- Implementation of User-User, Item-Item and Model Collaborative Filtering methods on the MovieLens Database.
- Locality Sensitive Hashing was used to speed up computation of Item-Item pairs
- Item-Item performs best with lowest `RMSE of 0.94`

Approximate running times:

- User-user: `600s`
- Item-item (with LSH): `400s`
- Model based: `14s`

__Note__: testing file must be a subset of input file and both should resemble the `ratings.csv` file on MovieLens Database
