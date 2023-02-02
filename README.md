# The Engage Corpus

The Engage Corpus is a large collection of posts and comments extracted from Reddit that can help researchers build large-scale, text-based recommender systems.

The publication associated with the Engage Corpus can be found [here](https://aclanthology.org/2022.lrec-1.200.pdf).

The Engage Corpus can be downloaded in 2 parts from the links below:

[reddit-data-01-part-01.tar.gz](https://drive.google.com/file/d/1F2SuyRUoC05mkmVNq9dektJpHzW3JkLd/view?usp=sharing)

[reddit-data-01-part-02.tar.gz](https://drive.google.com/file/d/1u81ji7m_McuMkIAA9v4jtAPi4ChKlBcp/view?usp=sharing)

To extract the dataset, run the following commands in Linux:

```
cat reddit-data-01-part-01.tar.gz reddit-data-01-part-02.tar.gz > reddit.tar.gz
tar -xzf reddit.tar.gz
```

Each line in the dataset contains the posts and comments of a single user in JSON format.

We show a hypothetical example from the dataset below:

```
{
  "user_number": 1202,
  "comments": [
    {
      "created_utc": 1552526370,
      "body": "Good effects, subpar writing. Clearly a showcase of the studio's VFX capabilities more than anything. Nothing wrong with that, just people should know going in that it's really just about the effects.",
      "id": "eih6cjm",
      "link_id": "t3_b0u22v",
      "score": 7,
      "subreddit": "scifi"
    },
    {
      "created_utc": 1574391764,
      "body": "I knew animals could have anxiety and stuff but I didn’t know about panic attacks. What does a cat panic attack look like?",
      "id": "f8a177i",
      "link_id": "t3_dzatoi",
      "score": 1,
      "subreddit": "Cats"
    }
  ],
  "posts": [
    {
      "created_utc": 1553035672,
      "title": "\'Gifted\' lemon-flavored pasta. What can I make with that?",
      "selftext": "I can ever only find how to make lemon-flavored pasta or a pasta dish with lemon included. I have no idea how to build or balance a dish with this ingredient. Thank you!",
      "id": "b3446p",
      "score": 2,
      "subreddit": "Cooking"
    },
  ]
}
```

If you found this work useful, please cite:

> Daniel Cheng, Kyle Yan, Phillip Keung, and Noah A. Smith. 2022. The Engage Corpus: A Social Media Dataset for Text-Based Recommender Systems. In Proceedings of the Thirteenth Language Resources and Evaluation Conference, pages 1885–1889, Marseille, France. European Language Resources Association.

Questions may be directed to the corresponding authors at d0@uw.edu, kyleyan@uw.edu, and pkeung@uw.edu.
