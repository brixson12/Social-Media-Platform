Simple Social Media Platform
This is a simple command-line based social media platform program implemented in Python. It allows users to post links, upvote links, post comments on links, and upvote comments. The program demonstrates basic functionalities of a social media platform in a simplified manner.

Features
Post a Link: Users can add new links with URLs and titles.
Upvote a Link: Users can increase the upvote count for a specific link.
Post a Comment: Users can add comments to existing links.
Upvote a Comment: Users can upvote comments associated with a specific link.
How to Use
Clone the Repository
bash
Copy code
git clone https://github.com/your-username/social-media-platform.git
cd social-media-platform
Run the Program
bash
Copy code
python social_media_platform.py
Interact with the Program
Follow the prompts in the command-line interface to perform actions such as posting links, upvoting links, adding comments, and upvoting comments.
Program Structure
social_media_platform.py: Contains the main program implementing the social media platform logic.
README.md: This file, providing information about the program.
LICENSE: License information (e.g., MIT License).
Sample Usage
python
Copy code
# Create an instance of the social media platform
social_media = SocialMediaPlatform()

# Post some links
link1 = social_media.post_link("https://example.com/article1", "Article 1")
link2 = social_media.post_link("https://example.com/article2", "Article 2")

# Upvote a link
social_media.upvote_link(1)

# Post comments on a link
social_media.post_comment(1, "Great article!")
social_media.post_comment(1, "Interesting!")

# Upvote a comment
social_media.upvote_comment(1, 1)

# Display all links with their details
all_links = social_media.get_all_links()
for index, link in enumerate(all_links, start=1):
    print(f"Link {index}: {link.title} - URL: {link.url} - Upvotes: {link.upvotes}")
    if link.comments:
        print("   Comments:")
        for i, comment in enumerate(link.comments, start=1):
            print(f"      Comment {i}: {comment.text} - Upvotes: {comment.upvotes}")
    else:
        print("   No comments yet")
    print()
License
This project is licensed under the MIT License - see the LICENSE file for details.

