# Reddit Api

An Api Client to download images (posts) from a certain subreddit corresponsding to certain keywords.

### Prequisites

1. A Reddit account
2. Reddit OAuth Credentials (get them [here](https://ssl.reddit.com/prefs/apps/))
3. [Optional] Gfycat API credentials (get the [here](https://developers.gfycat.com/signup/#/apiform))

### Usage

```
reddit = reddit_api.generate_instance_with_gfy("reddit_client_id","reddit_client_secret","user_agent","reddit_username","reddit_password","gfy_id","gfy_secret")

# or without gif links

reddit_api.generate_instance("reddit_client_id","reddit_client_secret","user_agent","reddit_username","reddit_password")

posts,matching_titles,matching_comments=reddit.get_posts("subreddit_name",["keyword_1","keyword_2"],limit]

```
